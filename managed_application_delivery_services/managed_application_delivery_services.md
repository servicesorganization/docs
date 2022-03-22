---
title:  Managed Application Delivery Services
#tags: [Liquit Workspace, Application Delivery]
keywords: Managed Application Delivery Services, MAD, Liquit Workspace
#last_updated: March 3, 2022
#summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: managed_application_delivery_services-sidebar
permalink: managed_application_delivery_services.html
folder: managed_application_delivery_services
YouTubeId: cszpDeo0aDk
MicrosoftStreamId: 1efb2e36-2641-4f79-af3d-a2f5d9636c7c
MicrosoftOnedriveId: s!AhPPtD3NKDurh-poYEbNgbHBgkRWJw?e=CnmWe8

---


## Managed Application Delivery Services

Hello World!

# Header 1
## Header 2
### Header 3
#### Header 4

Bullit points
- bullit 1
    - subbullit 1
    - subbullit 2
        - SubSubBullit
- bullit 2

![](attachments/ApplicationLifeCycle.png)

[About Liquit Workspace](mad_about_liquit_workspace.md)


{% include note.html content="Ik ben heel benieuwd" %}
{% include tip.html content="This is my tip. All the content I type here is treated as a single paragraph." %}
{% include important.html content="This is my important. All the content I type here is treated as a single paragraph." %}
{% include warning.html content="This is my warning. All the content I type here is treated as a single paragraph." %}

{% include youtubePlayer.html id=page.YouTubeId %}

{% include MicrosoftStream.html id=page.MicrosoftStreamId %}


PowerShell Code example
``` powershell
[System.Reflection.Assembly]::LoadWithPartialName(“System.Windows.Forms”)

[STRING]$Command = "[Windows.Forms.MessageBox]::Show(`“test`”, `“Ictworkspace.wordpress.com by Roel Beijnes`”, [Windows.Forms.MessageBoxButtons]::OK, [Windows.Forms.MessageBoxIcon]::Information)"

& "$env:windir\syswow64\windowspowershell\v1.0\powershell.exe" -noprofile -WindowStyle hidden -NonInteractive -executionpolicy bypass -command $Command
Write-Output "test"

```
