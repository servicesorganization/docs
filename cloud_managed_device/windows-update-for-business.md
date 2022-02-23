---
title: Windows Update for Business
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: windows-update-for-business.html
folder: cloud_managed_device
---

With Windows Update for Business, Windows client devices will be kept up-to-date with the latest security defenses and Windows features by directly connecting these systems to Windows Update service from Microsoft. With Microsoft Intune you configure update rings and settings to control when security updates are installed. It is also possible to control the feature updates (upgrade to a higher level of Windows) or stay at a certain Windows version.

<table data-layout="default" data-local-id="48f62fbc-b94b-47bd-9a13-51790662fae5" class="confluenceTable"><colgroup><col style="width: 82.0px;"><col style="width: 297.0px;"><col style="width: 380.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p>&nbsp;</p></td><td class="confluenceTd"><p>Two Windows update rings will be created:</p><ol><li><p>Fast ring (pilot ring)</p></li><li><p>Production ring</p></li></ol></td><td class="confluenceTd"><p>Two update rings will be created an assigned. One update ring will be assigned to user who will receive the updates as soon as possible. The second update ring will be receiving the updates after a period of time.</p></td></tr></tbody></table>

Delivery Optimization
=====================

Windows Update Delivery Optimization works by letting you get Windows updates and Microsoft Store apps from sources in addition to Microsoft, like other PCs on your local network, or PCs on the internet that are downloading the same files. Delivery Optimization also sends updates and apps from your PC to other PCs on your local network or PCs on the internet, based on your settings. Sharing this data between PCs helps reduce the internet bandwidth that’s needed to keep more than one device up to date or can make downloads more successful if you have a limited or unreliable Internet connection.

When Windows downloads an update or app using Delivery Optimization, it will look for other PCs on your local network (or from the internet, depending on your settings) that have already downloaded that update or app. Windows doesn’t download the entire file from one place. Instead, the download is broken down into smaller parts. Windows then gets parts of the update or app from the PCs that have it, and parts from Microsoft. Windows uses the fastest, most reliable download source for each part.

Delivery Optimization creates a local cache, and stores files that it has downloaded in that cache for a short period of time.

<table data-layout="default" data-local-id="35b87a95-b56c-4e70-8845-146635f16d3f" class="confluenceTable"><colgroup><col style="width: 82.0px;"><col style="width: 297.0px;"><col style="width: 380.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p>&nbsp;</p></td><td class="confluenceTd"><p>A Delivery Optimization device configuration profile will be created to set the Delivery Optimization settings for Windows</p></td><td class="confluenceTd"><p>To control the best practice delivery optimization settings on Windows, a policy must be created and assigned to the Windows devices.</p></td></tr></tbody></table>