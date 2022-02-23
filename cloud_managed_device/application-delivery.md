---
title: Application Delivery
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: application-delivery.html
folder: cloud_managed_device
---

Microsoft Store for Business
----------------------------

The Microsoft Store for Business is a portal where to find and purchase apps for the organization individually, or in volume. By connecting the store to Microsoft Intune, you can manage volume-purchased apps from the portal. For example:

*   You can synchronize the list of apps that have been purchased (or that are free) from the store with Intune.
    
*   Apps that are synchronized appear in the Intune administration console; you can assign these apps to users or devices like other apps.
    
*   Both Online and Offline licensed versions of Apps are synchronized to Intune. App names will be appended with "Online" or "Offline" in the portal.
    
*   You can track how many licenses are available, and how many are being used in the Intune administration console.
    
*   Intune blocks assignment and installation of apps if there are an insufficient number of licenses available.
    
*   Apps managed by Microsoft Store for Business will automatically revoke licenses when a user leaves the enterprise, or when the administrator removes the user and the user devices.
    

Intune Company portal
---------------------

The Intune Company Portal app, is where users access company data and can do common tasks. Common task may include enrolling devices, installing apps, and locating information. Additionally, they allow users to securely access company resources. The end-user experience provides several different pages, such as Home, Apps, App details, Devices, and Device details. To quickly find managed apps within the Company Portal, you can filter the apps on the Apps page.

Win32 apps
----------

Microsoft Intune allows Win32 app management capabilities. Although it's possible for cloud-connected customers to use Microsoft Endpoint Configuration Manager for Win32 app management, Intune-only customers will have greater management capabilities for their Win32 apps.

**Note:** When you're deploying Win32 apps, consider using the Intune Management Extension approach exclusively, particularly when you have a multiple-file Win32 app installer. If you mix the installation of Win32 apps and line-of-business apps during AutoPilot enrollment, the app installation might fail. The Intune management extension is installed automatically when a PowerShell script or Win32 app is assigned to the user or device.

Microsoft 365 apps
==================

By selecting Microsoft 365 apps for Windows 10/11 devices in Intune, you can assign and install Microsoft 365 apps to devices you manage that run Windows. You can also assign and install apps for the Microsoft Project Online desktop client and Microsoft Visio Online Plan 2, if you own licenses for them. The available Microsoft 365 apps are displayed as a single entry in the list of apps in the Intune console.

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 80.0px;"><col style="width: 307.0px;"><col style="width: 372.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The Microsoft Store for Business will be connected to Microsoft Intune.</p></td><td class="confluenceTd"><p>To manage the volume purchased apps in Intune, the Microsoft Store for Business will be connected to Microsoft Intune.</p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The Windows Store Intune company portal will be installed on every Windows device.</p></td><td class="confluenceTd"><p></p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>Microsoft 365 apps will be installed on every Windows device</p></td><td class="confluenceTd"><p>All devices will be installed with the Microsoft Office 365 apps like Word, Excel, Outlook, Powerpoint.</p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The Win32 Remote Help app will be installed on Windows devices</p></td><td class="confluenceTd"><p>To give support to end-users the remote app, currently in public preview, will be installed on all Windows devices.</p></td></tr></tbody></table>