---
title: Azure Log Analytics Update Compliance
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: azure-log-analytics-update-compliance.html
folder: cloud_managed_device
---


With Azure log analytics update compliance you can:

*   Monitor security, quality, and feature updates for Windows 10 or Windows 11 (professional, education or enterprise editions only)
    
*   View a report of device and update issues related to compliance that need attention.
    
*   Check bandwidth savings incurred across multiple content types by using Delivery Optimization.
    

Update Compliance must be configured through the Azure portal and no costs will be charged when using Azure log Update Compliance.

Update Compliance uses Windows client diagnostic data for all the reporting. Update compliance collects system data including:

*   Update deployment progress,
    
*   Windows Update for Business configuration data
    
*   Delivery Optimization usage data
    

The collected data will be send to the configured Azure Log Analytics workspace.

![](attachments/2014380248/2015789061.png)

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 80.0px;"><col style="width: 307.0px;"><col style="width: 372.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>Windows devices will be enrolled in Windows Log Analytics Update Compliance</p></td><td class="confluenceTd"><p>To monitor the Windows update and the delivery optimization, devices will be added to a update compliance portal.</p></td></tr></tbody></table>