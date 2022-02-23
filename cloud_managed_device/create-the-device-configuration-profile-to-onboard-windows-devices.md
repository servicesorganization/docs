---
title: Create the Device Configuration Profile to Onboard Windows Devices
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: create-the-device-configuration-profile-to-onboard-windows-devices.html
folder: cloud_managed_device
---


### Onboard Windows devices

After you connect Intune and Microsoft Defender for Endpoint, Intune receives an onboarding configuration package from Microsoft Defender for Endpoint. You use a device configuration profile for Microsoft Defender for Endpoint to deploy the package to your Windows devices.

The configuration package configures devices to communicate with Microsoft Defender for Endpoint services to scan files and detect threats. The device also reports its risk level to Microsoft Defender for Endpoint based on your compliance policies.

After onboarding a device using the configuration package, you don't need to do it again.

In the fallowing steps we will explain how to make this configuration,

1.  Sign in to the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431).
    
2.  Select **Endpoint security** > **Endpoint detection and response** > **Create Policy**.
    
3.  For **Platform**, select **Windows 10 and Later**.
    
4.  For **Profile type**, select **Endpoint detection and response**, and then select **Create**.
    
5.  On the **Basics** page, enter a _Name_ and _Description_ for the profile, then choose **Next**.
    
6.  On the **Configuration settings** page, configure the following options for **Endpoint Detection and Response**:
    
    *   **Sample sharing for all files**: Returns or sets the Microsoft Defender for Endpoint Sample Sharing configuration parameter.
        
    *   **Expedite telemetry reporting frequency**: For devices that are at high risk, **Enable** this setting so it reports telemetry to the Microsoft Defender for Endpoint service more frequently.
        
7.  Select **Next** to open the **Scope tags** page. Scope tags are optional. Select **Next** to continue.
    
8.  On the **Assignments** page, select the groups that will receive this profile.
    
    Select **Next**.
    
9.  On the **Review + create** page, when you're done, choose **Create**. The new profile is displayed in the list when you select the policy type for the profile you created. **OK**, and then **Create** to save your changes, which creates the profile.