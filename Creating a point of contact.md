---
title: Creating a point of contact
layout: layout-page-sidenav
description: This article explains how to provision your Yealink deskphone using assisted provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Creating a point of contact
redirect_from:
    - https://support.ringcentral.com/article-v2/Creating-a-point-of-contact.html?brand=RingCentral&product=CC&language=en_US
---

### Creating a point of contact

A point of contact (POC) is an entry point, such as a phone number or email address, that an inbound contact uses to initiate an interaction. The POC works side-by-side with skills and Studio scripts to route contacts according to your custom handling rules. You can assign multiple POCs to a single skill or script, but you can only assign one skill and one script to each POC.
For example, a contact may call one of several toll-free numbers to reach your organization. Each of those numbers is a different path to enter the Contact Center system. You can create different contact points for each number and associate each number with a routing script and skill to guide the agents who receive the interaction.
You can create POCs for the following channels:
**Chat:** POCs for the chat channel are automatically assigned identifiers. You can associate a chat profile with a POC to control the interface customers will see when chatting.
**Email:** POCs for the email channel can be associated with any email address from which you want to route emails to your agents.
**Phone call:** POCs for a phone call can be associated with any phone number at which you want to receive calls that you then route to your agents. Each phone number must be configured in your call center by RingCentral Contact Center’s Professional Services team before you can associate it with a POC.
**SMS:** POCs for SMS (text messaging) is associated with any number at which you want to receive SMS messages that you then route to your agents.
**Work items:** POCs for the “work items” channel are automatically assigned identifiers. You can create different POCs for work items from different sources.
**How to create a point of contact**
Sign in to RingCentral Contact Center.
Navigate to Applications > ACD.
Click Points of Contact.

Click Create New, then select Single Point of Contact.

Click the Media Type dropdown. You can select Chat, Email, Phone Call, SMS, or Work Item.

Enter a name in the Name field.
Click the Point of Contact dropdown and select an available number. You can order additional numbers if none are listed.
Click the Skill dropdown and select the skill that you want to handle the calls that are routed through this POC.
Click the Script dropdown and select the phone script that you want to handle the calls that are routed through this POC.
Check the IVR Reporting Enabled box if you wish to enable this feature.
Click the Chat Profile dropdown if you’ve selected Chat in the Point of Contact dropdown. Select your preferred Chat Profile from the list.

Click Create Point Of Contact.
Your new POC will appear in your Points of Contact list.
