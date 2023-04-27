---
title: Intro to deskphone provisioning | RingCentral MVP
layout: layout-page-sidenav
description: This article explains how to use the provisioning process to connect a deskphone to RingCentral servers.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title:  Intro to deskphone provisioning
redirect_from:
    - https://support.ringcentral.com/article-v2/intro-deskphone-provisioning.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Intro to deskphone provisioning | RingCentral MVP

A deskphone — sometimes called an internet phone or a broadband phone — is a standalone, internet-ready device that uses Voice over Internet Protocol (VoIP) to make and receive calls.
Before you can use a deskphone with your VoIP provider, make sure you provision it. 

Provisioning connects your deskphone to RingCentral’s VoIP servers so you can use it for secure calling, audio conferencing, and online meetings.

There are two ways to connect your deskphones to RingCentral’s servers:

Deskphones purchased directly from RingCentral are preconfigured to connect automatically.

Deskphones that you already own or have purchased from a third-party vendor must be provisioned to connect. This option is known as Bring Your Own Device (BYOD). See the complete list of third-party deskphones that are compatible with RingCentral.

**Purchasing deskphones from RingCentral**

RingCentral sells many VoIP deskphones, all of which are preconfigured to connect to our servers. Deskphones purchased directly from RingCentral don’t require provisioning.

**Provisioning Bring Your Own Device (BYOD) deskphones**

If your existing deskphones are on the list of compatible devices, you can provision and use them with your RingCentral account.

**Before provisioning any BYOD deskphone**

Before provisioning any third-party deskphone to work with your RingCentral account:

1) Confirm your deskphone is compatible with RingCentral .

2) Make sure the deskphone is unlocked. You can contact its vendor to verify how to unlock it or learn whether it’s unlocked.

3) Make sure you have RingCentral admin access. If you aren’t sure:
Go to the Admin Portal and sign in. Click Users in the top menu, then Roles in the left navigation bar. 
Look for User Admin or Super Admin under Role Name.

4) Confirm your deskphone meets RingCentral’s network requirements .

5) Perform a factory reset of your deskphone. We recommend you delete all of your deskphone’s existing configurations before connecting it to your RingCentral account. The process for factory resets differs by manufacturer.
Factory reset for Cisco phones
Factory reset for Mitel phones
Factory reset for Poly phones
Factory reset for Yealink phones

6) Check which types of provisioning your deskphone supports. The three types are assisted, manual, and Zero Touch. Refer to the complete list of compatible BYOD devices to see which types of provisioning your deskphone supports.

7) Confirm your deskphone has been assigned a local number or DigitalLine . Note: RingCentral doesn’t recommend provisioning a single device with multiple DigitalLines. Using multiple DigitalLines on a single phone can cause connection issues.

**Assisted provisioning**
Assisted provisioning is available for most deskphones that RingCentral sells and supports. The general steps are:

1) Locate your deskphone’s serial number. Serial numbers, sometimes called MAC addresses, are often located on stickers on the back of devices. If you can’t locate the serial number, contact the manufacturer.

2) Enter your deskphone’s serial number into the Admin Portal.

3) Enter RingCentral’s provisioning server address into your deskphone’s menu.
The assisted provisioning process differs by manufacturer.
Assisted provisioning for Cisco phones
Assisted provisioning for Mitel phones
Assisted provisioning for Poly phones
Assisted provisioning for Yealink phones
Once you’ve set up your deskphone with assisted provisioning, it will connect automatically to RingCentral’s servers. Updates and new features will be downloaded to it automatically.

**Manual provisioning**
If your deskphone doesn’t support assisted provisioning, you can use manual provisioning. To do this, find and enter your Session Initiated Protocol (SIP) settings.
Manual provisioning has some limitations. Manually provisioned devices:
Can’t receive automatic updates from RingCentral’s servers.
Can’t receive RingCentral firmware updates.
Can’t use RingCentral’s Presence feature.
Don’t have softkeys for Paging or Intercom features.
The manual provisioning process differs by manufacturer.
Manual provisioning for Cisco phones
Manual provisioning for Mitel phones
Manual provisioning for Poly phones
Manual provisioning for Yealink phones

**Zero Touch Provisioning (ZTP)**
Deskphones that support ZTP can be provisioned automatically.
Before you use ZTP:
Perform a factory reset of your deskphone.
If you’re using a deskphone that you’ve used with a different provider and it was connected to that provider using ZTP, you may need to disconnect the device’s MAC address, or serial number, from its previous ZTP setup.
For most phones, you’ll need to request that your previous provider delete your phone’s MAC address from their servers.
For Poly phones, email Poly’s ZTP support (ztpinfo@poly.com) to request a transfer of the device’s MAC address to RingCentral. To bypass the ZTP process for Poly phones, you can use assisted provisioning.
