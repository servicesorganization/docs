---
title:  Configure Device Enrollment
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: configure-device-enrollment.html
folder: cloud_managed_device
---
To configure Intune Device Enrollment:

1.  Sign in to the [Endpoint Manager portal](https://endpoint.microsoft.com)
    
2.  Go to **Devices => Windows => Windows enrollment => Automatic Enrollment**
    
3.  Set MDM user scope to **All**
    
4.  Set the following URL’s:
    
    *   MDM terms of use URL: [https://portal.manage.microsoft.com/TermsofUse.aspx](https://portal.manage.microsoft.com/TermsofUse.aspx)
        
    *   MDM discovery URL: [https://enrollment.manage.microsoft.com/enrollmentserver/discovery.svc](https://enrollment.manage.microsoft.com/enrollmentserver/discovery.svc)
        
    *   MDM compliance URL: [https://portal.manage.microsoft.com/?portalAction=Compliance](https://portal.manage.microsoft.com/?portalAction=Compliance)
        

Example:
--------

![](attachments/2012348435/2012217737.png)