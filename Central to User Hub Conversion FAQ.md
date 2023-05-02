---
title: Central to User Hub Conversion FAQ
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Central to User Hub Conversion FAQ
redirect_from:
    - https://support.ringcentral.com/article-v2/Central-to-User-Hub-Conversion-FAQ.html?brand=RingCentral&product=CC&language=en_US
---

### Central to User Hub Conversion FAQ

**Why is it called “conversion” instead of “migration”?**
Migration implies moving or copying data from one place to another. This process does not copy any data. It simply changes the sign-in process and admin interface.
**Will conversion be done on a whole cluster or by Business Unit (BU)?**
All conversions are based on BU. Each BU is converted separately.
**How long does it take to convert from Central to User Hub?**
The entire conversion process lasts one to three hours. The team should plan to be engaged in this for up to an hour for the conversion itself (and any adjustments and retries) and an hour or two after for post-conversion tasks. While the conversion itself takes up to 30 minutes, there is preparation to ensure a seamless conversion. The multi-week preparation includes a dedicated RingCentral team who will work with you to examine your environment and create a mutual project plan to deliver a successful outcome.
The time it takes is based on the size of the Business Unit (BU) and more specifically, on the number of users, teams, and security profiles. BUs with over 1,000 agents should discuss the expected time frame with their Project Lead once they are assigned to the conversion.
**Will my contact center be unavailable during the conversion process?**
There will be some downtime associated with the conversion process. The IVR will continue to function and contacts will be routed. Contacts in queue will remain that way, and more contacts can be queued.
Your conversion will happen between 8 AM and 5 PM local time on your determined conversion date. During that time, up to 200 agents may remain logged in. Calls will continue to be routed to agents, and any scheduled reports during that time frame will continue to run. Depending on the size of your system, the estimated duration will be up to 30 minutes.
**Do agents need to be signed out during the conversion process?**
Up to 200 Agents can remain signed in and will continue to receive contacts. However, their session token refreshes hourly, and if it expires during the conversion, they may not be able to automatically refresh, meaning that they will be down until the process finishes.
If agents are signed in when the conversion process finishes, they should sign out and sign back in again. If they do not, their session will expire one hour after the conversion process has been completed and they will be signed out automatically.
**What if agents are actively handling a contact when the conversion starts?**
Active contacts will continue without interruption and each agent will be able to finish the contact and disposition it as normal. We recommend that agents set their next state to Unavailable, then sign out and sign back in once the current contact has been handled.
**Where is my data located after conversion?**
We are not copying any data as part of the conversion. All data will remain in the same location.
**I use the RingCentral Contact Center ACD recorder and File Server to record calls and store the recordings. Will this work the same way after conversion?**
Yes. The ACD recorder will continue to work exactly as it did before, and no files will be changed or lost during the conversion process. You will also access the recordings exactly as you did before.
**I recently migrated files from RingCentral Contact Center File Server to Storage Services. Does the conversion process change how this works?**
No. The conversion process does not change how you use Storage Services, and it will continue to work exactly as it did before conversion.
**Will any changes be made to scripts or points of contact?**
No. All scripts and points of contact will remain unchanged.
**I use multi-factor authentication and hardware tokens. Will they continue to work after conversion?**
Yes. User Hub supports MFA and tokens using TOTP and HOTP.
**Will the way I sign in change after conversion?**
Yes. The link you use to sign in will change from ringcentral.incontact.com to ringcentral.nice-incontact.com. Bookmarks for the sign-in page should be updated once the conversion process has been completed.
**What happens if I attempt to sign in using the old URL after conversion?**
An update has been deployed that will check to see whether your username has been converted to User Hub. If you are part of a Business Unit (BU) that has been converted, the sign-in process will automatically redirect to the new URL while preserving your username.
**Will passwords be the same after conversion?**
No. As part of the conversion process, every user will have their password reset since we do not have the ability to read a user's password. When the user signs in again for the first time, they will be prompted to change their password.
**Will Agent for Salesforce continue to work after conversion?**
Yes. However, you will need to ensure you have downloaded and installed the latest version of the application into Salesforce. You will receive further instructions during the implementation process.
**Can I migrate inactive users who are assigned to inactive teams or security profiles?**
No. All users must be moved to active teams and security profiles prior to conversion.
