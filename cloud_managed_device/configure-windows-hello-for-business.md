---
title:  Configure Windows Hello for Business
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: configure-windows-hello-for-business.html
folder: cloud_managed_device
---

1.  Sign in to the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431).
    
2.  Go to **Devices** > **Enrollment** > **Enroll devices** > **Windows enrollment** > **Windows Hello for Business**.
    
3.  Apply the following settings:
    
    *   Configure Windows Hello for Business: **enabled**
        
    *   Use a Trusted Platform Module (TPM): **required**
        
    *   Minimum PIN length: **6**
        
    *   Maximum PIN length: **127**
        
    *   Lowercase letters in PIN: **Not allowed**
        
    *   Uppercase letters in PIN: **Not allowed**
        
    *   Special characters in PIN: **Not allowed**
        
    *   PIN expiration days: **never**
        
    *   Remember PIN history: **5**
        
    *   Allow biometric authentication: **No**
        
    *   Use enhanced anti-spoofing, when available: **Yes**
        
    *   Allow phone sign-in: **Yes**
        
    *   Use security keys for sign-in: **Enabled**
        
4.  Click **Save**