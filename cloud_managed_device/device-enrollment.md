---
title: Device Enrollment
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: device-enrollment.html
folder: cloud_managed_device
---

Intune lets you manage your company or personal devices and apps and how they access your company data. To use this mobile device management (MDM), the devices must first be enrolled in the Intune service. When a device is enrolled, it's issued an MDM certificate. This certificate is used to communicate with the Intune service.

<table data-layout="default" data-local-id="5d0404e1-f67f-4ce9-974d-e50e4d345ad3" class="confluenceTable"><colgroup><col style="width: 81.0px;"><col style="width: 301.0px;"><col style="width: 378.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p>DD01</p></td><td class="confluenceTd"><p>The Automatic enrollment will be set to the default MDM URLs</p></td><td class="confluenceTd"><p>To enroll devices in Intune, the default Terms of use, MDM discovery and MDM compliance URLs must be published.</p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The MDM user scope will be set to All</p></td><td class="confluenceTd"><p>The MDM autoenrollment will be set to allow all devices or users.</p></td></tr></tbody></table>

By default, devices for all platforms are allowed to enroll in Intune. However, you can restrict devices by platform and a maximum a user can enroll.

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 81.0px;"><col style="width: 303.0px;"><col style="width: 376.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The Windows MDM corporate enrollment restrictions will be allowed. Personally owned devices will be blocked to enroll</p></td><td class="confluenceTd"><p>Corporate Windows enrollment will be allowed to use Windows Autopilot to enroll a device. Personally owned devices will be blocked to enroll in Intune.</p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The number of devices a user can enroll will be set to a maximum.</p></td><td class="confluenceTd"><p>A maximum will limit the number of devices a user can enroll</p></td></tr></tbody></table>