---
title: Install Agent Adapter for Salesforce in Lightning Experience | RingCentral Contact Center
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Install Agent Adapter for Salesforce in Lightning Experience | RingCentral Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/10704-Agent-Adapter-for-Salesforce-Lightning-Experience-RingCentral-Contact-Center.html?brand=RC_US&product=RingCentral_Contact_Center&language=en_US
---

### Install Agent Adapter for Salesforce in Lightning Experience | RingCentral Contact Center

This article describes the steps when you install the RingCentral Contact Center Agent Adapter for Salesforce - Lightning.
Note : This article does not apply to Engage customers.
The Agent Adapter for Salesforce uses the Lightning Open CTI connector and supports the Salesforce Lightning Experience desktop environment in conjunction with the Salesforce Classic environment. The Lightning Experience interface includes contextual hover capabilities, a contact history feed, record details, and related lists. For help using or troubleshooting the Lightning Experience, see the Salesforce help for Finding Your Way Around Lightning .
**Install Agent Adapter for Salesforce in Lightning Experience**
Log into the Salesforce org where you want to install the Agent Adapter for Salesforce.
Click on the App Launcher (upper left corner, beside Setup).
On the pop-up window, click Visit AppExchange on the upper right corner of the page.
Search for NICE inContact then click on the App.
User-added image
5. Click Get it Now .
User-added image
Follow the installation prompts, choosing the settings applicable to the business need.
**Build a Lightning App to use Agent Adapter for Salesforce in Lightning Experience**
In the Lightning Experience view, click Setup .
Under Platform Tools, click Apps > App Manager .
Click New Lightning App .
Add app details and click Next .
Select Standard navigation and click Next .
Click Add > Open CTI Softphone .
Add a new label, or leave the default label, and click Next .  No need to alter the panel scaling.
Click an item and the right arrow to add it to your new app. After adding the items you want, click Next .
Click a profile name and the right arrow to assign the app to the profile. After assigning the app to the appropriate profiles, click Save & Finish.  Your newly created app now appears in the App Launcher and the App Manager.
Launch your new app.
**Troubleshooting**
If the Phone icon for Salesforce Agent does not show in the Lightning Console, follow these steps:
Click here to open the lightning config file.xml
Right-click the page then click on Save As .  
Save the File on a location on your computer.  This will be imported in Salesforce.
On the Call Center page in Salesforce, select the import button.
Choose the downloaded file from its saved location on your machine.
Move the agents from the old Call Center to the new one you just created.
This should be done after hours as to not interrupt any agents who are logged into the application.
If an agent is logged in when this is done, have them log out and back in to their Salesforce instance (not just the Agent application).
The 'Phone ' button should now be visible.
See also:
Agent Adapter for Salesforce - Overview | RingCentral Contact Center
Agent Adapter for Salesforce - Update Agent Adapter for Salesforce | RingCentral Contact Center
Agent Adapter for Salesforce - Install Agent Adapter for Salesforce Classic View | RingCentral Contact Center
