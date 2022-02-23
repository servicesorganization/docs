---
title: Encryption of Data
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: encryption-of-data.html
folder: cloud_managed_device
---

OneDrive uses advanced data-encryption methods between your device and the Microsoft data center. At rest, OneDrive uses disk encryption through BitLocker Drive Encryption and file encryption to secure your data. Each file is encrypted with its own encryption key; anything larger than 64 KB is split into individual chunks, each of which has its own encryption key locked in a key store.

Each file chunk is then randomly distributed among Microsoft Azure Storage containers, and a construction map for the complete file is stored in a separate secure content database. For attackers to access the file, they would need all the file chunks, the keys, and the map—a highly improbable task.