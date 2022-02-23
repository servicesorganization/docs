---
title:  What is a Cloud Managed Device
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: 01-what-is-a-cloud-managed-device.html
folder: cloud_managed_device
---

The question which is asked a lot of times by customers is “Everyone is talking about a Modern Workplace but what exactly is this Modern Workplace or Cloud Managed Device and why is my current Workplace not modern?”.

As you know a lot of companies are moving workloads to the Microsoft cloud, you can think of Exchange Online, Skype Online, SharePoint Online, OneDrive for Business, etc. All these tools are modern and can easily secure with Azure MFA and other security features like Conditional Access which are available within the Microsoft Cloud.

However, a lot of data is still synchronized from a traditional Windows device (think of OneDrive Data, SharePoint Data, Exchange Data, etc.), joined to the local Active Directory which resides in an in house or public datacenter. So, we can secure the Microsoft cloud while we’re not fully in control of the sensitive data on the end user device and besides that, the data is stored within a different ‘domain’ than the ‘domain’ where the device resides of the end user.

The Modern Workplace is not the solution for all these issues, but it works better with all modern tools available within the Microsoft Cloud as it resides within the same ‘domain’. This Modern Workplace will, therefore, be joined to the Azure Active Directory where it will be managed by Intune. Within Intune, we can specify compliance rules which the end user device must match before the device will get ‘compliant’. If a device isn’t compliant, we can revoke access to all synchronized items such as Outlook, OneDrive, etc. This will force the user either to get their device compliant but still gives him or her the ability to work but web-based for the time being.

Besides all the above we also can remotely wipe the device within Intune, meaning getting more control over the company data and devices which aren’t always connected to the internal network.