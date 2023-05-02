---
title: Hours of Operation Overview | RingCentral Contact Center
layout: layout-page-sidenav
description: This article explains how to provision your Yealink deskphone using assisted provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Hours of Operation Overview | RingCentral Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/11298-Hours-of-Operation-Overview-RingCentral-Contact-Center.html?brand=RC_US&product=RingCentral_Contact_Center&language=en_US
---

### Hours of Operation Overview | RingCentral Contact Center

This article describes the purpose of creating Hours of Operation profiles. Hours of operation profiles allow you to configure business hours within the system, both for normal scenarios and special scenarios like holidays, seasonal periods, etc.

For more videos like this, visit RingCentral University.
 
Note : This article does not apply to Engage customers.
 
**Hours of Operation Overview**
Hours of operation profiles allow you to configure business hours within the system, both for normal scenarios and special scenarios like holidays, seasonal periods, etc.
When you set up hours of operation, the platform auto-generates a profile ID that you apply to the  HOURS  action in Studio. Studio actions determine workflow and routing for the channels and types of contacts in your system. The HOURS action enables the workflow to differ based on the hours of operation profile. For example, the system can send the contact to an agent's queue (if your business is open) or tell the contact to call back (if your business is closed).
You can alternatively set up hours of operation profiles directly in Studio (see  Set an Hours of Operation Profile in Studio ).
If you have different hours for different departments, you can set up multiple hours of operation profiles and then assign the skills associated with each department to the appropriate profile. A skill can only belong to one hours of operation profile.
 
**Override Branches**
There may be times when your organization needs to override normal contact routing. For example, inclement weather or a natural disaster may force a closure of your facility. Override branches provide a quick way to change your hours of operation profile temporarily, without making changes directly to your script or creating an entirely new profile.
The system provides for these override branches:  Weather ,  Meeting ,  Emergency , and  Other . To use any of these, you must have a matching branch configured in your Studio contact routing script(s). If you invoke an override, and there is no corresponding Studio branch, contacts follow the default branch.
You cannot invoke an override branch while creating a new profile.
You configure an expiration date and time for the override at the time you invoke it. If you do not set an expiration, the override remains in effect until it is turned off manually.
 
**Related Tasks**
Set Up an Hours of Operation Profile
Assign Skills to an Hours of Operation Profile
Edit or Delete an Hours of Operation Profile
Override the Normal Hours of Operation
Set an Hours of Operation Profile in Studio
Edit an Hours of Operation Profile in Studio
Delete an Hours of Operation Profile in Studio
