---
title:  Create Windows health monitoring template
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: 01-create-windows-health-monitoring-template.html
folder: cloud_managed_device
---

1.  Sign in to the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431).
    
2.  Select **Devices** > **Configuration profiles** > **Create profile**.
    
3.  Enter the following properties:
    
    *   **Platform**: Choose **Windows 10 and later**.
        
    *   **Profile**: Select **Templates** > **Windows health monitoring**
        
4.  Select **Create**.
    
5.  In **Basics**, enter the following properties:
    
    *   **Name**: Enter a name for the profile.
        
    *   **Description**: Enter a description for the profile. This setting is optional, but recommended.
        
6.  Select **Next**.
    
7.  In **Configuration settings**, configure the following settings:
    
    *   **Health monitoring**: Select **Enable**
        
    *   **Scope**: Select:
        
        *   **Windows updates**: This option configures devices to send Windows Update data to Intune. This data is then used in a [compliance policy](https://docs.microsoft.com/en-us/mem/intune/protect/windows-update-compliance-reports) that reports on Windows updates.
            
        *   **Endpoint analytics**
            
8.  Select **Next**.
    
9.  Select **Next**.
    
10.  Select **Next**.
    
11.  Select **Next**.
    
12.  Select **Create**,
    

![](attachments/2014675062/2014937173.png)