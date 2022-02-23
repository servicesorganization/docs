---
title: Security Baselines
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: security-baselines.html
folder: cloud_managed_device
---

Intune makes it easy to deploy Windows security baselines to help you secure and protect your users and devices.

Even though Windows is designed to be secure out-of-the-box, many organizations still want more granular control over their security configurations. To navigate the large number of controls, organizations often seek guidance on configuring various security features. Microsoft provides this guidance in the form of security baselines.

Security baselines are groups of pre-configured Windows settings that help and enforce granular security settings that are recommended by the relevant security teams. It is possible to customize each baseline to enforce only those settings and values the company requires. When you create a security baseline profile in Intune, you're creating a template that consists of **multiple _device configuration_ profiles.**

You deploy security baselines to groups of users or devices in Intune, and the settings apply to devices that run Windows 10/11. For example, the _MDM Security Baseline_ automatically enables BitLocker for removable drives, automatically requires a password to unlock a device, automatically disables basic authentication, and more. When a default value doesn't work, customize the baseline to apply the settings the company wants.

Separate baseline types can include the same settings but use different default values for those settings. It's important to understand the defaults in the baselines, and to then modify each baseline to fit your organizational needs.

Security baselines can help to have an end-to-end secure workflow when working with Microsoft 365. Some of the benefits include:

*   A security baseline includes the best practices and recommendations on settings that impact security. Intune partners with the same Windows security team that creates group policy security baselines. These recommendations are based on guidance and extensive experience.
    
*   If you're new to Intune, and not sure where to start, then security baselines gives you an advantage. You can quickly create and deploy a secure profile,
    
*   If you currently use group policy, migrating to Intune for management is much easier with these baselines. These baselines are natively built in to Intune, and include a modern management experience.
    

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 80.0px;"><col style="width: 297.0px;"><col style="width: 382.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The latest Microsoft Security Baseline will be applied on all devices.</p></td><td class="confluenceTd"><p>The Microsoft Security Baseline for Windows 10 will be applied on the Windows devices and serve as a guideline.</p></td></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The latest Microsoft Defender for Endpoint baseline will be applied on all devices</p></td><td class="confluenceTd"><p>The Microsoft Defender for Endpoint will be applied on the Windows devices and serve as a guideline.</p></td></tr></tbody></table>