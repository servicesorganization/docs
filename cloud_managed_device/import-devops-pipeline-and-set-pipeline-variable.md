---
title: Import Devops Pipeline and Set Pipeline Variable
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: import-devops-pipeline-and-set-pipeline-variable.html
folder: cloud_managed_device
---

Import a DevOps pipeline
------------------------

To run a pipeline, first we have to create the pipeline.

*   Open [https://dev.azure.com/](https://dev.azure.com/dwswanalytics/)
    
*   Select the project
    
*   Select Pipelines
    
*   Click **…** (after Create Pipeline) and select Import Pipeline
    
*   Browse to the Pipeline file (JSON file) and click Open.
    

![](attachments/2024636417/2025914399.png)

*   Click on **Import**
    
*   In DevOps, select **Azure Pipelines** as Agent Pool and **Windows-latest** as Agent Specification
    

![](attachments/2024636417/2025881651.png)

*   Click **Get sources**
    
*   Select the **Team Project** and **Repository**
    

![](attachments/2024636417/2025914441.png)

*   Click Save & queue
    
*   Click **Save**
    

Add App Registration Variable groups
------------------------------------

*   Select **Library**
    
*   Click **\+ Variable Group**
    
*   Type **DevOpsIntune App registration** as **Variable Group name**
    
*   Type a Description (optional)
    
*   Click **+Add**
    
*   Add the following Variables:
    

<table data-layout="default" data-local-id="b5592a02-e229-4f12-a7a6-4e4e6f0cdec3" class="confluenceTable"><colgroup><col style="width: 340.0px;"><col style="width: 340.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>Name</strong></p></th><th class="confluenceTh"><p><strong>Value</strong></p></th></tr><tr><td class="confluenceTd"><p>tenantId</p></td><td class="confluenceTd"><p>[Directory (tenant) ID</p></td></tr><tr><td class="confluenceTd"><p>client_id</p></td><td class="confluenceTd"><p>[Application (client) ID</p></td></tr><tr><td class="confluenceTd"><p>client_secret</p></td><td class="confluenceTd"><p>Secret value</p></td></tr></tbody></table>

*   Insert the tenantID
    
*   Insert the cliend\_id
    
*   Insert the client\_secret
    

![](attachments/2024636417/2025881667.png)

*   Click on **Save**
    

  
Add Customer Variable Group
------------------------------

*   Select **Library**
    
*   Click **\+ Variable Group**
    
*   Type **CustomerGroup** as **Variable Group name**
    
*   Type a Description (optional)
    
*   Click **+Add**
    
*   Add the following Variables:
    

<table data-layout="default" data-local-id="0caa5698-0e14-4cbc-92a8-f49ab8027b32" class="confluenceTable"><colgroup><col style="width: 340.0px;"><col style="width: 340.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>Name</strong></p></th><th class="confluenceTh"><p><strong>Value</strong></p></th></tr><tr><td class="confluenceTd"><p>CompanyName</p></td><td class="confluenceTd"><p>Example: Orange</p></td></tr><tr><td class="confluenceTd"><p>Country</p></td><td class="confluenceTd"><p>Example: NLD</p></td></tr><tr><td class="confluenceTd"><p>DeviceName</p></td><td class="confluenceTd"><p>Example: LT- for laptops, or KIOSK- for Kiosk devices</p></td></tr><tr><td class="confluenceTd"><p>DeviceType</p></td><td class="confluenceTd"><p>Example: Laptop</p></td></tr></tbody></table>

*   Insert the Company Name
    
*   Insert the Country or Region
    
*   Insert the DeviceName used for Autopilot enrollment
    
*   Insert the DeviceType
    

![](attachments/2024636417/2025947190.png)

*   Click on **Save**
    

Link the variable groups to the pipeline
----------------------------------------

*   Open [https://dev.azure.com/](https://dev.azure.com/dwswanalytics/)
    
*   Select the project
    
*   Select Pipelines
    
*   Click **Edit** the Pipeline
    
*   Click **Variables**
    
*   Click **Variable Groups**
    
*   Click **Link variable group**
    
*   Select **DevOpsIntune App registration** and click **Link**
    
*   Click **Link variable group**
    
*   Select **CustomerGroup** and click **Link**
    
*   Click Save & queue
    
*   Click **Save**
    

![](attachments/2024636417/2025848882.png)