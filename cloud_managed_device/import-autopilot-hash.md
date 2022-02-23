---
title:  Import Autopilot Hash
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: import-autopilot-hash.html
folder: cloud_managed_device
---

Step 1: create a device hardware hash
-------------------------------------

1.  On the Windows device open a powershell (admin) console
    
2.  Type: **Set-ExecutionPolicy Bypass**
    
3.  Type: **Install-Script -Name Get-WindowsAutopilotInfo**
    
4.  Type: **Get-WindowsAutoPilotInfo.ps1 -OutputFile \[path\]\\\[name\].csv**
    

![](attachments/2012709144/2012709171.png)

Step 2: Import the Windows Autopilot hash:
------------------------------------------

1.  Sign in to the [Endpoint Manager portal](https://endpoint.microsoft.com/)
    
2.  Go to **Devices => Windows => Windows enrollment => Devices**
    
3.  Click on **Import**
    
4.  Select the csv file
    
5.  Click on **Import**
    

![](attachments/2012709144/2012872824.png)