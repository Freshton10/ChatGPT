---
title: Assisted provisioning for Mitel deskphones
layout: layout-page-sidenav
description: This article explains how to provision your Mitel deskphone using assisted provisioning.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Assisted provisioning for Mitel deskphones
redirect_from:
    - https://support.ringcentral.com/article-v2/assisted-provisioning-mitel-deskphones.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Assisted provisioning for Mitel deskphones

**Before provisioning your Mitel deskphone**

Make sure your Mitel deskphone supports assisted provisioning. If your phone isn’t on the list, go to Manual provisioning for third-party (BYOD) Mitel phones to set it up. Mitel deskphones must be of a minimum revision (REV) level to use assisted provisioning with the RingCentral platform. Learn more about Mitel hardware requirements for RingCentral compatibility.
Make sureyour deskphone has been assigned a local number or DigitalLine. The MAC address of your phone can’t be assigned to a user who’s been removed from your system. It must be assigned to either an active user, or a user marked as Not Activated.
If you purchased your deskphone from a different provider, make sure it’s unlocked before you proceed. You can contact the provider to learn whether it’s unlocked or how to unlock it.
Make sure your network is configured according to RingCentral’s network requirements.
Verify open access on port 443 (https) to the RCS (ZTP) server by whitelisting the following URL or IP address:
Rcs.aastra.com
216.191.234.139
Verify open access on port 443 by whitelisting the following URLs:
mtl.ringcentral.com (provisioning)
mtl.s3.ringcentral.com (firmware update)
If you’re migrating devices from a legacy Mitel platform, verify the removal of any DHCP / DNS entries in the environment that might redirect the Mitel phones to the old platform.
Common legacy Mitel DHCP / DNS entries:
If DHCP Option 156 is configured, it must be removed prior to migrating the phone(s).
Ensure the following configuration does not appear anywhere for DHCP or LLDP: configservers=update.sky.shoretel.com, CloudDomain=sky.shoretel.com 
Any Mitel-specific DNS values in DHCP will cause the migration to fail; commonly these are 208.103.94.230 and 199.101.107.70.  
Test the zero-touch provisioning/assisted provisioning of several phones from various network sites ahead of cutover. This will verify if the network is set up correctly.
 
**Provisioning an existing deskphone to a Mitel phone**

Go to the Admin Portal and sign in.
Select Phone System in the top menu.
Go to Phones & Devices > User Phones. Find the device with the DigitalLine or phone number that you want to assign to your Mitel deskphone, then click its name from the Device column.
Click Setup & Provision.

Enter Mitel in the search bar. Select your device when its full name appears.

Click Next.
Enter the phone’s MAC address and click Next.

Follow the instructions in the Setup & Provisioning window.
Click Done.
Reboot your deskphone to register it with RingCentral’s network.
 
**Provisioning an existing RingCentral Phone app to a Mitel deskphone**

If you selected RingCental Phone app when you created or added a new user, and you want to change it to use a Mitel deskphone, follow the steps below.
Go to the Admin Portal and sign in.
Select Phone System in the top menu.
Go to Phones & Devices > User Phones.
Select the existing RingCentral phone app from the list that you want to assign to your Mitel deskphone and click its name from the Device column.
Click Change Phone.

Add Emergency Response Location. You can add either a Company emergency response location or Other location.
Click Next.
Enter Mitel in the search bar. Select your device when its full name appears.

Click Next.
Enter the phone’s MAC address and click Next.

**Follow the instructions in the Setup & Provisioning window.**

Click Done.
Switch your RingCentral Phone to the new extension. Open the RingCentral Phone on the appropriate computer and edit the login settings to the new extension.
Reboot your Mitel deskphone to register it with RingCentral’s network.
