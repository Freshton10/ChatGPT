---
title: Call Delay Issues with Australia | RingCentral Contact Center
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Call Delay Issues with Australia | RingCentral Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/10044.html?brand=RC_US&product=RingCentral_Contact_Center&language=en_US
---

### Call Delay Issues with Australia | RingCentral Contact Center

This article provides troubleshooting steps for resolving call delay issues encountered in phones located in Australia contact centers.
Note : This article does not apply to Engage customers.
Call delays are encountered.
A possible cause may be due to network issues.
Another possible cause of the call delay is due to the phones registering to the Singapore DC when Australian Contact Center Agent Pattern was set to use a United States Contact Center Agent Pattern. This causes approximately 3 seconds of delay in the call.
Resolve network issues
Check if your system passes the requirements: RingCentral Contact Center Platform Requirements
Use this tool to isolate the QoS issue: Troubleshooting QoS Issues with the PingPlotter Tool
 
Resolve location registration issues
Change your Agent Pattern from US to APAC Agent Dial string. 
Global Prefix Pattern:
GlobalPrefixRange   CountryCode MainNumber  * EXT
Agent Pattern
User Assigns Agent Pattern to Own User Profile
User hovers over the left panel then clicks the Name.
User clicks Edit then select the Pattern under Default Dialing.  
 
User-added image
Global Prefix Routing on Studio Script
Common case is a hunt group on the RingCentral side. The call is coming to contact center and option 3 directs to hunt group.  The call is redirected to RC using TAS Engage pseudonumber.
 
User-added image
 
Another example in this script, BEGIN triggers the HOURS action. If the Hours of Operation profile settings show the contact center to be open, the call will be delivered to an agent. If the contact center is closed or on holiday, BLINDXFER will route the call to 999702441970629143*8030  (set in the BLINDXFER properties) to be transferred to a RingCentral Extension.
 
User-added imagey
