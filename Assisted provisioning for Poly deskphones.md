---
title: Assisted provisioning for Poly deskphones
layout: layout-page-sidenav
description: This article explains how to use assisted provisioning to connect Poly deskphones to RingCentral’s servers, with special instructions for Poly IP deskphones and the Poly OBi302 VoIP Gateway.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Assisted provisioning for Poly deskphones
redirect_from:
    - https://support.ringcentral.com/article-v2/assisted-provisioning-poly-deskphones.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Assisted provisioning for Poly deskphones

**Before you provision your Poly deskphone**

1. Make sure it’s compatible with RingCentral and that it supports assisted provisioning .
If your deskphone isn’t compatible with RingCentral, you won’t be able to use it with your RingCentral service.
If your deskphone is compatible with RingCentral but doesn’t support assisted provisioning, you’ll need to connect it with manual provisioning.

2. Confirm that it meets RingCentral’s network requirements.
3. Confirm that it has been assigned a local number or DigitalLine.
4. If you purchased your device from a different provider, make sure the phone is unlocked . If you’re unsure, contact Poly Customer Support.
5. Make sure you’re a RingCentral admin with permission to make changes to Phones & Devices.
6. Perform a factory reset of your Poly deskphone. We recommend that you delete all of your deskphone’s existing configurations before connecting it to your RingCentral account.

**Provisioning your Poly deskphone**
Note: If you’re connecting a Poly OBi302 VoIP Gateway, follow the alternate provisioning instructions for that device.
 
1. Go to the Admin Portal and sign in.
2. Select Phone System in the top menu.
3. Go to Phones & Devices > User Phones . Select the device with the DigitalLine or phone number that you want to assign to your Poly deskphone and click its name in the Device column.
click its name in the Device column
4. On the next screen, click Set Up and Provision .
click Set Up and Provision
5. In the Setup & Provisioning window, begin typing the name of your Poly deskphone, then scroll to find it in the dropdown. When you locate your deskphone, click its name, then click Next.
Note: If you can’t locate the name of your deskphone in the dropdown, you’ll need to set it up using manual provisioning by clicking Set up manually using SIP. Learn more about manual provisioning for Poly deskphones
type the name of your Poly deskphone
6. Locate your deskphone’s MAC address, or serial number, and enter it into the field on the Provisioning window. (A device’s MAC address is typically located on its underside.) Click Next.
Note: If you’re provisioning a Poly deskphone with “IP” in its model name, continue to Assisted provisioning for Poly IP deskphones.
Provisioning window
7. Follow the Manual Configuration Instructions in the Finish window. You’ll perform a factory reset on your deskphone, then connect it to RingCentral’s servers. When you’ve completed all the steps, click Done.
Note: Your deskphone will restart, then automatically provision itself to connect to RingCentral’s servers. It will also download any updates and/or new features.

**Assisted provisioning for Poly IP deskphones**

Poly deskphones that have “IP” in their model names require a special provisioning process. After you’ve completed the first six steps in Provisioning your Poly deskphone, continue to the following steps.

1. On your deskphone, press the Menu key (or softkey), then go to Settings > Advanced > Admin Settings > Network Configuration > Provisioning Server > DHCP Menu.
2. From the DHCP Menu, select Boot Server and change the setting to Static.
3. Click OK, then select Back.
4. Go to Server Menu > Server Type. Enter the following:
Server Type: HTTPS
Server Address: pp.ringcentral.com/pp
Server User: <blank>
Server Password: <blank>
Note: Use the << softkey or the X key to delete any existing values. Use number keys to enter letters. For example, to enter a, press 2 once; to enter c, press 2 three times; to enter a period, press *; to enter a slash, press # several times.
5. Select OK to accept changes.
6. Select Back to save your configuration, and select Back again to exit.
7. Select OK. Your phone will restart.
Once your phone has restarted, click Done in the Setup & Provisioning window in the Admin Portal.

**Assisted provisioning for Poly OBi302**
The Poly OBi302 VoIP Gateway is an adapter that lets you connect an analog phone to RingCentral’s VoIP servers. It requires a special provisioning process.

**Before provisioning the Poly OBi302**
You’ll need:
Your OBi302 device and its power adapter
An ethernet cable
Access to your internet router
A DigitalLine for the user extension that will use this device. If you don’t have one, read about how to assign a DigitalLine.

**Installing the Poly OBi302**

1. Connect your analog phone to the green Phone 1 port.
2. Plug one end of the ethernet cable into the blue Internet port, then plug the other end into an open port on your internet router, modem, or ethernet switch.
Plug in the OBi302.
Plugging OBi302
3. Turn on the OBi302’s web interface.
4. Pick up your phone’s handset. (You won’t hear a dial tone.)
Enter ***0
Enter 30#
Enter 1
Enter 1#
Enter 1 to save
Note: By default, Wide Area Network (WAN) access is turned off.
5. Go to the Admin Portal and sign in.
6. Select Phone System in the top menu.
7. Go to Phones & Devices > User Phones . Select the device with the DigitalLine or phone number that you want to assign to your Poly deskphone and click its name in the Device column.
8. click its name in the Device column
On the next screen, click Set Up and Provision .
click Set Up and Provision
In the Select Device tab, enter “obi,” then select Polycom OBi302 ATA when it appears in the dropdown. Click Next.
select Polycom OBi302 ATA
In the Provisioning tab, follow the instructions for provisioning the OBi302. The general steps are:
Obtain the device’s IP address
Locate the device’s MAC address (typically on its underside)
Perform a factory reset
Enter the MAC address in the Admin Portal
Access the device’s web interface
Configure the provisioning server
Disable WAN access on your device (if it hasn’t already been disabled)
Save your new configuration
When you’ve completed all steps, the OBi302 will restart. It’ll automatically provision itself to connect to RingCentral’s servers.
