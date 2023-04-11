---
title: Manual provisioning for Linksys PAP2-NA-ATA | RingCentral MVP
layout: layout-page-sidenav
description: This article will guide you on configuring your Cisco Linksys PAP2-NA ATA via manual provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Manual provisioning for Linksys PAP2-NA-ATA 
redirect_from:
    - https://support.ringcentral.com/article-v2/How-to-provision-a-Linksys-PAP2-NA-ATA.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Manual provisioning for Linksys PAP2-NA-ATA | RingCentral MVP

 Before proceeding with the manual provisioning, you need to first retrieve the manual SIP configuration settings from the online account. Once you have the settings, follow the steps below:

1. Plug an Ethernet cable from the router's Ethernet port to the Linksys PAP2-NA ATA.

2. Get the device’s IP address by going through the phone menu:

Dial * four (4) times

Dial 110# and take note of the IP address
 
3. On your computer, launch your web browser then enter the IP address in the address bar.

4. Click on Admin Login.

5. User-added image

6. Click on switch to advanced view.

7. User-added image

8. Click on the Line 1 tab.

9. User-added image

10. Enter the SIP configuration information you have obtained from the online account. The User ID is also the RingCentral DigitalLine number, and the Password and Authentication ID is always the same.

11. Auth ID, Block CID Serv, Dist Ring Serv should be set to yes.

12. User-added image

13. Click on Save Settings.  The device will automatically reboot and the settings on the IP phone will be updated.
