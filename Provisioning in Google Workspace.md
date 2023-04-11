---
title:Activating Auto User Provisioning in Google Workspace into RingCentral
layout: layout-page-sidenav
description: This article provides instructions for setting up and activating Google Workspace Auto User Provisioning (Google Cloud Directory) for your RingCentral account.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Activating Auto User Provisioning in Google Workspace into RingCentral
redirect_from:
    - https://support.ringcentral.com/article-v2/10587-G-Suite-Auto-User-Provisioning.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Activating Auto User Provisioning in Google Workspace into RingCentral

**Google Auto User Provisioning enables** IT admins to provision G Suite / Google Workspace users into RingCentral automatically. This simplifies user management between Google Workspace and RingCentral. 

When an IT admin creates, modifies, or deletes users in Google Workspace, they are correspondingly updated in their RingCentral service.

1. Sign in to G Suite / Google Workspace Admin console .
2. Navigate to Apps > SAMLapps . 
3' Select RingCentral on the list of SAML apps. To set up the RingCentral SAML app, visit  Setting up Single Sign-On (SSO) for Google in RingCentral Admin Portal .
4. Under Autoprovisioning , click ConfigureAutoprovisioning .
5. Click Authorize .
6. Enter your RingCentral login credentials to verify authorization. 
7. Map RingCentral user attributes to corresponding Cloud Directory attributes, and then click Next . 
**Note: You can set up custom address attributes after if you haven’t mapped it out.**

1. Click Continue .
2. Select the groups you want to include in the Autoprovisioning. (Optional)
3. Click Continue .
4. Set up your Deprovisioning settings.
5. Click Finish .
 
Note: Changes may take up to 24 hours to propagate to all users.
If users exceed the admin authorized account seat limit, users will not be assigned. An error prompt will be shown in Google Workspace until the admin adds more users to the RingCentral account. 
The users auto-created in RingCentral will be capped by the number of seats/users purchased in RingCentral. Attempting to auto-provision more users into RingCentral than the number of seats/users purchased will be flagged as an error in the Google Workspace provisioning dashboard. 
Admin will need to purchase the appropriate number of seats/users in RingCentral to match the estimated number of provisioned users from Google Workspace.
