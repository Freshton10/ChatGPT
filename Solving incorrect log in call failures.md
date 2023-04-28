---
title: Solving incorrect log in call failures
layout: layout-page-sidenav
description: This article explains how to provision your Yealink deskphone using assisted provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Solving incorrect log in call failures
redirect_from:
    - https://support.ringcentral.com/article-v2/Solving-incorrect-log-in-call-failure.html?brand=RingCentral&product=CC&language=en_US
---

### Solving incorrect log in call failures

When inbound calls fail to reach an agent, often the cause involves incorrect login information (username, station ID, phone number, etc.). As a result, the following may occur:
Inbound calls will not ring on the MAX agent application.
No calls will route to the agent.
Calls will route to the incorrect agent to solve the problem.
Agents will not receive calls on their desk phones.
Agents will be locked out of their account.
**Causes**
An incorrect login can occur on two platforms agents utilize: either the desktop platform or the phone application.
Desktop platform: Agents who use softphone application on their computer input the wrong information (username, password, phone #), resulting in receiving no calls from customers.
Phone application: Agents taking calls on a deskphone input their station ID or phone number incorrectly so no calls will route to their physical device.
**Resolution**
**How to check login credentials**
If agents can't receive phone calls on their softphone or deskphone, they should check that all credentials, specifically their station ID or phone number, are correctly entered. Oftentimes, these two cause the inbound calls to not route to the agent because they’re incorrect.
**Troubleshooting password reset attempts by agents**
If an agent is unable to log in, they may attempt to reset/update their password. In some instances, an error message may still appear stating that either their password or username is incorrect. In these cases, administrators will need to perform the following to assure the user is listed as “active”:
Log in to RingCentral Contact Center.
In the left-hand navigation, click Employees.

You will now see a list of the Employees. There are 3 states the employees will fall under:
If the user is in a state of "Invite"; you can click on that button and this will send an invite to the user's configured email address in order to give them access.
Once the "Invite" is selected and sent, the user will be placed in a "Pending" state, which means the system is waiting for a response to the "Invite" sent.
Once the user is sent the invite and accepts the invite and logs into CXone, the user will now be in an "Active" state.

If the user is in a Pending state as shown above, but for some reason did not get the Invite notification via email, you can tick the box next to the users name. 
Once the checkbox is checked the Invite button on the top right-hand corner of the page will light up. 
Once the user is selected, click Invite. The system will send out another invite to the users configured email address.
Sometimes, the Pending status will expire. If this is the case, click the triangle with an exclamation point inside of it. This will open a window that will give the option of re-sending the invite to the user. 
Click Resend to invite the user.

**Resetting user passwords for Central via Manage Users**
You can manage your RingCentral Contact Center Users in the Admin application. This article provides instructions on how to reset a user's password.
Log in to RingCentral Contact Center.
Go to Admin > Users.
Click the user’s name.
On the General tab, click Reset Password.
Type in a new password and click Done.
An email notification will be sent to the user with the new password. Note: The instructions above are only applicable for Central Account in RingCentral Contact Center, not for UserHub.
