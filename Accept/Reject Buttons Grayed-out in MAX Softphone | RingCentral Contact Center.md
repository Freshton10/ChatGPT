---
title: Accept/Reject Buttons Grayed-out in MAX Softphone | RingCentral Contact Center
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Accept/Reject Buttons Grayed-out in MAX Softphone | RingCentral Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/Accept-Reject-Buttons-Grayed-out-in-MAX-Softphone-RingCentral-Contact-Center.html?brand=RC_US&product=RingCentral_Contact_Center&language=en_US
---

### Accept/Reject Buttons Grayed-out in MAX Softphone | RingCentral Contact Center

This article provides a quick workaround for resolving the grayed-out accept/reject buttons in MAX softphone.
**NOTE :** This article does not apply to Engage customers.
 
Accept button is greyed-out, unable to pick up calls when using MAX softphone.
 
MAX Integrated Softphone
Chrome version 88 and 89
We’ve identified a new feature that Chrome first introduced as being Enabled by default in Version 88. This new feature affects web pages in tabs that are minimized or set behind another window (occluded) for 5 or more minutes of inactivity. When these requirements are hit, Chrome heavily throttles timers running in Javascript. 
**Currently Available Workaround:**
Type this in the address bar - chrome://flags
Disable this Chrome flag (then search for “throttle” as seen below), as a possible workaround.
**throttle**
 
After the Throttle Javascript Timers flag has been disabled, you may also need to Clear cache & cookies
Depending on the microphone device used by the agent, they may have to go to Chrome Settings, search for “Site Settings,” then find and expand “Microphone.” Once there, you will update the device option to Communications (as seen below) Selecting instead of using Default ensures the device is chosen correctly every time.
**device**
As an alternative to changing this flag & settings, agents can try to ensure that MAX remains open in the “foreground,” which means they do not minimize it or put any other windows over the top of it.
We realize and understand that this is not always ideal; and we are working to get a better, long term solution identified and implemented as quickly as possible.
**UPDATE TO CHROME VERSION 90:**
With the release of Chrome version 90, Javascript throttling is no longer an experimental flag and it is now under the IntensiveWakeUpThrottling Chrome policy outlined here:
https://chromeenterprise.google/policies/?policy=IntensiveWakeUpThrottlingEnabled
The throttling issue causing the problems outlined in this article are addressed in RingCentral Contact Center release 21.1.4 which begins deployment in late April 2021. While waiting for 21.1.4 to be released to your cluster, we encourage you to either hold off on upgrading to Chrome 90 or disable IntensiveWakeUpThrottling via Chrome Enterprise Policies.
