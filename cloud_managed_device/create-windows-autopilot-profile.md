---
title:  Create Windows Autopilot Profile
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: create-windows-autopilot-profile.html
folder: cloud_managed_device
---

To create a Windows autopilot profile:

1.  Sign in to the [Endpoint Manager portal](https://endpoint.microsoft.com/)
    
2.  Go to **Devices => Windows => Windows enrollment => Windows Autopilot deployment profiles**
    
3.  Click on **Create profile**
    
4.  Select **Windows PC**
    
5.  Type a profile name (required) and description (optional)
    
6.  Select **Convert all target devices to Autopilot** to **Yes**
    
7.  Click **Next**
    
8.  In the Out-of-box-experience (OOBE) select:
    
    *   Deployment mode: **User-Driven**
        
    *   Join to Azure AD as: **Azure AD joined**
        
    *   Microsoft Software License Terms: **Hide**
        
    *   Privacy settings: **Hide**
        
    *   User account type: **Standard**
        
    *   Allow White Glove OOBE: **Yes**
        
    *   Language (Region): **Operating system default**
        
    *   Automatically configure keyboard: **No**
        
    *   Apply device name template: **Yes**
        
    *   Enter a name: **\[variable\]-%RAND:5%**
        
9.  Click **Next**.
    
10.  In the Scope tags, click **Next**.
    
11.  On the Assignments, click **Next**.
    
12.  Click on **Create**
    

![](attachments/2012676181/2012610674.png)![](attachments/2012676181/2012840052.png)