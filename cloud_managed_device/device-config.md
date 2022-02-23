---
title: Device Config
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: device-config.html
folder: cloud_managed_device
---

Device profiles allow you to add and configure settings, and then push these settings to devices. You have some options when creating policies:

*   **Administrative templates**: On Windows 10 and later devices, these templates are ADMX settings that you configure. If you're familiar with ADMX policies or group policy objects (GPO), then using administrative templates is a natural step to Microsoft Intune and Endpoint Manager.
    
*   **Baselines**: On Windows 10 and later devices, these baselines include preconfigured security settings. If you want to create security policy using recommendations by Microsoft security teams, then security baselines are for you.
    
*   **Settings catalog**: On Windows 10 and later devices, use the settings catalog to see all the available settings, and in one location. For example, you can see all the settings that apply to BitLocker, and create a policy that just focuses on BitLocker.
    
*   **Templates**: On Android, iOS/iPadOS, macOS, and Windows devices, the templates include a logical grouping of settings that configure a feature or concept, such as VPN, email, kiosk devices, and more. If you're familiar with creating device configuration policies in Microsoft Intune, then you're already using these templates.