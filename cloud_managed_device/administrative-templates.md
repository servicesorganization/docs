---
title: Administrative Templates
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: administrative-templates.html
folder: cloud_managed_device
---
When managing devices, you want to create groups of settings that apply to different device groups. For example, you have several device groups. For GroupA, you want to assign a specific set of settings. For GroupB, you want to assign a different set of settings. You also want a simple view of the settings you can configure.

You can complete this task using Administrative Templates in Microsoft Intune. The administrative templates include thousands of settings that control features in Microsoft Edge version 77 and later, Internet Explorer, Microsoft Office programs, remote desktop, OneDrive, passwords, PINs, and more. These settings allow group administrators to manage group policies using the cloud.

The Windows settings are similar to group policy (GPO) settings in Active Directory (AD). These settings are built in to Windows, and are ADMX-backed settings that use XML. The Office and Microsoft Edge settings are ADMX-ingested, and use the ADMX settings in Office administrative template files and Microsoft Edge administrative template files. And, the Intune templates are 100% cloud-based. They offer a simple and straight-forward way to configure the settings,

Administrative Templates are built in to Intune, and don't require any customizations, including using OMA-URI. As part of your mobile device management (MDM) solution, use these template settings as a one-stop shop to manage your Windows devices.

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 80.0px;"><col style="width: 307.0px;"><col style="width: 372.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The Administrative template will be used to configure custom settings.</p></td><td class="confluenceTd"><p>Custom settings will be applied to set default configurations for example automatically sign-in to OneDrive for Business or automatically sign-in to Microsoft Outlook when Microsoft Outlook is started the first time.</p></td></tr></tbody></table>