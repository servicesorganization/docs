---
title: Azure App Registration and Api Permissions
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: azure-app-registration-and-api-permissions.html
folder: cloud_managed_device
---

Add App registration
--------------------

*   Sign in to [https://portal.azure.com](https://portal.azure.com)
    
*   Open **Azure Active Directory**
    
*   Click **App registration**
    
*   Click **New registration**
    
*   Type a name for the app registration (for example DevOpsIntune)
    
*   Select: **Accounts in this organizational directory only (Single tenant)**
    
*   Click **Register**
    

![](attachments/2024669255/2024445211.png)

Add secret
----------

*   Click **Certificates & secrets**
    
*   On the **Client Secrets** tab, click **\+ New client secret**
    
*   Type a description
    
*   Select the expiration
    
*   Click **Add**
    
*   **Important:** Save the secret Value (Secret ID).
    

![](attachments/2024669255/2024543409.png)

API Permissions
---------------

*   Click API Permissions
    
*   Click **Add a permission**
    
*   Select **Microsoft Graph**
    
*   Select **Application permissions**
    
*   Add DeviceManagementApps.ReadWrite.All
    
*   Add DeviceManagementConfiguration.ReadWrite.all
    
*   Add DeviceManagementManagedDevices.ReadWrite.All
    
*   Add DeviceManagementServiceConfig.ReadWrite.All
    
*   Add Group.Create
    
*   Click **Add permissions**
    
*   Click **Grant admin consent for \[tenant name\]**
    
*   Click Yes
    

![](attachments/2024669255/2025783297.png)

Get the Application (client)ID, Directory (tenant) ID:
------------------------------------------------------

*   Click on **Overview**
    
*   Save the Application (client) ID and Directory (tenant) ID:
    

![](attachments/2024669255/2024603743.png)