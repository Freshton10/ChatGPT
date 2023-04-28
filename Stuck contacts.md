---
title: Stuck contacts
layout: layout-page-sidenav
description: This article explains how to provision your Yealink deskphone using assisted provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Stuck contacts
redirect_from:
    - https://support.ringcentral.com/article-v2/Stuck-Contacts.html?brand=RingCentral&product=CC&language=en_US
---

### Stuck contacts

Stuck contacts are defined as a contact (i.e., inbound call, chat, email, or voicemail) that never reaches an available agent. A stuck contact could occur due to the following reasons:
Two contacts arrive simultaneously, and one reaches an agent while another does not.
Server rollover causes a call to reach the platform right when the server turns over to back up.
We experience an issue on our end. For example, our system drops for some reason, and the contact ends before it gets to an agent.
An internet outage of any kind occurs.
You use a LOOP action in your Studio script and forget to add the FINISH branch.
It gets assigned to an invalid skill.
**Clearing a stuck contact**
Go to the RingCentral Contact Center. Log in using your credentials.
In the left side menu, click on Reporting.
Click on Prebuilt Reports.
Click on Active Contacts in the list. 
Active Contacts in Prebuilt Reports
Find the phone number that got stuck.  Note: defining a stuck contact varies by customer expectations
Click on the phone number in the Contact ID column.
A window will open. Click the Contact Options tab. 
Contact Options in Prebuilt Reports
Click Clear Contact.
Click OK. This will end the stuck contact call and allow the customer to redial, get into the queue, and reach an available agent.
Should this solution not work for your stuck contact issue, please reach out to our Professional Services team to put in a ticket. They will assist you with fixing it by performing a deep dive into the root of the problem.
