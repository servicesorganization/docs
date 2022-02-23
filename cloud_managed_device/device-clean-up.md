---
title: Device Clean-up
tags: [Intune]
keywords: groups, api, structure
last_updated: July 3, 2016
summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: cloud_managed_device-sidebar
permalink: device-clean-up.html
folder: cloud_managed_device
---

Intune has the feature to cleanup devices that are MDM enrolled. Devices that appear inactive, stale, or unresponsive for more than the configured set of days. Intune will immediately and continuously clean up so that your device records remain current.

<table data-layout="default" data-local-id="42a408eb-d7ea-4a09-96ce-d6c63dc82c95" class="confluenceTable"><colgroup><col style="width: 84.0px;"><col style="width: 313.0px;"><col style="width: 363.0px;"></colgroup><tbody><tr><th class="confluenceTh"><p><strong>#</strong></p></th><th class="confluenceTh"><p><strong>Decision</strong></p></th><th class="confluenceTh"><p><strong>Justification</strong></p></th></tr><tr><td class="confluenceTd"><p></p></td><td class="confluenceTd"><p>The device cleanup will be set to 180 days</p></td><td class="confluenceTd"><p>Device objects will be removed from the Intune portal after 180 days of inactivity.</p></td></tr></tbody></table>