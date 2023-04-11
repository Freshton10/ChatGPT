---
title: Manual provisioning for Cisco Cisco SPA-122 ATA | RingCentral MVP
layout: layout-page-sidenav
description: This article provides information for configuring a Cisco SPA-122 ATA via manual provisioning. [NOTE: RingCentral does not provide additional support for phones purchased from third-party vendors. For product support on devices not purchased from RingCentral, please refer to the product's vendor for support].
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title:  Manual Provisioning for Cisco and 3rd Party/BYOD phones
redirect_from:
    - https://support.ringcentral.com/article-v2/652.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Manual provisioning for Cisco Cisco SPA-122 ATA | RingCentral MVP

**Provisioning your Cisco SPA-122 ATA**

Make sure that the phone is unlocked before you proceed.

1.  Add a Local Phone Number  and assign it to the extension who will use the phone.
2.  Get the SIP Settings from your RingCentral Online account.
3. Get the ATA device's IP Address , then access the web interface. Refer to your phone's user guide if you need additional help. 
4. Click  **Admin Login** . You will be asked to enter the Admin username and password. The default settings are: 
Username:  admin
Password:  admin
5. Click  Advanced .
6. Go to  Voice , then click  Provisioning . Set the following under  Configuration Profile :
Provision Enable:  yes
Resync On Reset:  no
Profile Rule:  leave the field empty/blank.
7. Scroll down at the bottom of the page, and then  Submit All Changes . The ATA device will restart. You will need to access the ATA device's User Interface again to continue.
8. Go to  Voice , and then configure the following settings under  Line 1 . 
General
Line Enable:  yes
SIP Settings
SIP Port:  any number between 5060-5090
9. Scroll down and look for  Proxy and Registration , and then configure the settings below, using the  SIP information  from your RingCentral account. 
Proxy and Registration
Proxy:  sip.ringcentral.com
Outbound Proxy:  enter the Outbound Proxy from your  SIP information
Subscriber Information
Display Name:  specify the name that will appear on your phone for identification
Password:  enter the Password from your  SIP information  
Auth ID:  enter the Authorization ID from your  SIP information  
User ID:  enter the User Name from your  SIP information . 
Use Auth ID:  yes
10. Scroll down, and then click  Submit All Changes . 
[NOTE:  The ATA device will reboot several times during the provisioning process. DO NOT manually turn off / DO NOT unplug the device during this process. To know if the ATA device is  Online  after Manual Provisioning, log in to the RingCentral Online account , then go to Admin Portal > Phone System > Phones & Devices > User Phones . Your phone is Online when you see a green check User-added image  next to it.] 
