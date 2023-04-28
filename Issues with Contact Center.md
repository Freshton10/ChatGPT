---
title: Issues with Contact Center
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title:  Issues with Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/Issues-with-Contact-Center.html?brand=RingCentral&product=CC&language=en_US
---

### Issues with Contact Center

**Issues with signing in to Contact Center**
Invalid username and password: Users may get an Invalid Username and Password error when logging in to Central (even when they use a temporary password).
Typical causes: Browser issues, issues with user account settings, or corrupted user profiles.
Resolutions:
Clearing your browser cache.
Reset your password.
Modifying or deactivating, then reactivating, your user profile.
Agent not receiving Password Reset Email from Central: An agent is locked out of their agent interface and can’t receive the email that will help them reset their password.
Typical causes: Several settings on the agent’s side can cause this issue.
Resolutions:
Admins should verify the agent’s user settings to check their correct work email, and change and/or reset their password.
Receiving an error message for Forget Password Email: Agents may receive this error message when they click the link in the email that instructs them how to reset their forgotten password.
Typical cause: The password-reset emails have expired.
Resolution: Configure your email client (Gmail, Outlook, etc.) to allow the domain (e.g. incontact.com / niceincontact.com) to bypass security scanning. This will prevent the email link from expiring.
Issues with a stuck contact or stuck agent
Agents stuck on ACW after completing a Personal Connection call:
Typical cause: This issue happens when an agent is unable to change their status back to Available after handling a call.
Resolution: Check if the automatic wrap-up state has an unavailable code set. If not, choose one from the dropdown.
Contact is stuck in Central Queue: Contacts from incoming calls, chat, or email can get stuck in the queue.
Typical cause: Internet outage, contact is assigned incorrectly to an invalid skill, a studio script is unfinished, the server rolls over, and/or simultaneous contacts entry.
Resolution: Learn how to clear a stuck contact.
Issues with call refusals or calls being put in a question, on hold, or timeouts
Inbound and outbound agent call refusals: Neither inbound nor outbound calls will connect, and display as refused.
Typical cause: If the number entered in the Station ID field for Caller ID is not valid, the system rejects the call delivery and then shows refused without routing the contact.
Resolution: Make sure you use a valid number as your Caller ID.
Agents are complaining about calls being delivered but are then refused.
Timeout settings on User Hub are 45 seconds by default: This error causes early and/or unintentional call refusal.
Typical cause: Short timeout settings cause unintentional call refusal.
Resolution: Go to the Contact Settings tab > Contact Refusal Timeouts > Contact Type. Adjust the contact type.
High volume of call refusals in MAX when using mobile phones: Agents experience a high volume of refused calls when using mobile phones. Agents may not even hear the phone ring before it gets refused.
Typical causes: Multiple causes.
Causes with workarounds: Mobile phone on silent mode, mobile phone is in power saving mode, mobile carrier returning a "ringing" or "session progress" response before actually alerting the mobile subscriber of the incoming call or taking too long to find the subscriber without returning a "ringing" or "session progress" response.
Causes without workarounds: Low to no mobile signal, carrier routing issues.
Resolution: Several factors cause this issue, which can be worked around and avoided. Causes without workarounds are suggested to be dealt with by the carrier. Causes with workarounds can be worked-on by
Preventing the mobile phone in standby mode,
Using WiFi calling,
Increase the timeout for no answer refusals to 36 seconds or more,
Ensuring the phone is not in silent mode and the ringer volume is set to a volume which can be heard
Disabling power saving mode or connect the mobile device to power.
