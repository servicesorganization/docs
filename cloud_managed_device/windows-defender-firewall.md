---
title: Windows Defender Firewall
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: windows-defender-firewall.html
folder: cloud_managed_device
---

If we’re managing your devices using Microsoft Intune, you may want to control your Windows Defender Firewall policy. A firewall controls what network traffic is allowed and not allowed to pass through ports. For regular devices like laptops and desktops, the firewall should allow little inbound traffic. There is rarely any legitimate reason for other devices to connect to your device, or home network, unsolicited. Therefore, it's important to have Microsoft Defender Firewall switched on to protect your device from unauthorized access.

![](attachments/2013495484/2014248987.png)

Picture of Devices firewall status,  
  
Tip#  
Microsoft defender Firewall settings are also applied in combination with Microsoft security baseline.

<table data-layout="default" data-local-id="48f62fbc-b94b-47bd-9a13-51790662fae5" class="confluenceTable"><colgroup><col style="width: 82.0px;"><col style="width: 297.0px;"><col style="width: 380.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p>&nbsp;</p></td><td class="confluenceTd"><p>Microsoft Firewall will be enabled for private and public profiles</p></td><td class="confluenceTd"><p>Every device gets the configuration settings that the Windows firewall will be enabled.</p></td></tr></tbody></table>