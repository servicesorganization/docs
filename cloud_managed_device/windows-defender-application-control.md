---
title: Windows Defender Application Control
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: indows-defender-application-control.html
folder: cloud_managed_device
---

With thousands of new malicious files created every day, using traditional methods such as antivirus solutions is an insufficient defense against new attacks. Windows Defender Application Control makes sure that apps are trusted unless they are blocked by an antivirus or other security solution. By using the "Code Integrity policy" of Windows Defender Application Control, it determines which applications are considered trusted.

![](attachments/2015723527/2015723534.png)

Windows Defender Application Control can be configured in two modes:

1.  **Enforcement enabled** - Only trusted executables are allowed to run.
    
2.  **Audit only** - Allow all executables to run, but log untrusted executables that run in the local client event log.
    

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 80.0px;"><col style="width: 307.0px;"><col style="width: 372.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>Windows Defender Application Control will be configured as Audit only. WDAC will <u>not be</u> configure as Enforcement enabled option.</p></td><td class="confluenceTd"><p>We do not want to block any not assigned application from running. If all business apps and applications are known, this setting can be changed to Enforcement enabled, but be careful because it can block apps or applications from running.</p></td></tr></tbody></table>