---
title: Agent Salesforce Install Issues under a Sandbox Environment | RingCentral Contact Center
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Agent Salesforce Install Issues under a Sandbox Environment | RingCentral Contact Center
redirect_from:
    - https://support.ringcentral.com/article-v2/Agent-Salesforce-Install-Issues-under-a-Sandbox-Environment-RingCentral-Contact-Center.html?brand=RC_US&product=RingCentral_Contact_Center&language=en_US
---

### Agent Salesforce Install Issues under a Sandbox Environment | RingCentral Contact Center

This article is to provide basic troubleshooting that resolves install issues under Salesforce Sandbox environment in RingCentral Contact Center.
**NOTE :** This article does not apply to Engage customers.
 
Unable to install the latest version of Agent for Salesforce sandbox environment.
 
Agent for Salesforce
RingCentral Contact Center
If you cannot install the latest version of Agent for Salesforce, the below steps may resolve the issue. 
Verify that the person trying to complete the update is a Salesforce admin. If not, that person will not be able to complete the update.
Check the Call Centers in your Salesforce instance. There are times that extra Call Centers are not needed, and it conflicts with the ones being updated in the new version. Delete any unused Call Centers and try to install the package again.
Refresh the sandbox from production to ensure your sandbox mirrors your production environment and try to install again.
In Salesforce, validate the permission Org Asset Library is enabled in the org. 
Uninstall the existing package from the sandbox and reinstall it.
