---
title: Manual provisioning for Yealink phones
layout: layout-page-sidenav
description: This article contains steps on how to provision your Yealink device manually.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Manual provisioning for Yealink phones
redirect_from:
    - https://support.ringcentral.com/article-v2/Manual-provisioning-Yealink-phones.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Manual provisioning for Yealink phones

To create a new user extension for your Yealink device, follow the steps below. If you want to provision your Yealink device manually for an existing user, go to Provisioning Yealink phones manually.
 
**Create a new user**
1. Log in to the RingCentral admin portal.
2. From the Admin Portal, navigate to Users > User List > Users with Extensions.
3. Click Add User. The Add Users window appears.
4. Select a Location from the dropdown list in Office User type, then click Select. 
5. Fill in the basic information about the user. Require unique email IDs is checked by default. You can uncheck it if you don’t want to invite users by email and use other user setup options.
6. If you’d like to add more users, enter the number on the field provided, then click Add.
Note: You can add up to 24 more users (25 users at a time). You may also click the duplicate icon at the far right to create a new row, and retain the selection details.  All details except the first name, last name, and email will be included.

7. Under Phone, select Bring your own device.
8. Under Number, use the dropdown menu to select a number to be assigned to your Yealink device. 
9. Click Done after selecting the number. 
10. Click Next.
11. Choose how you’d like to set up the new user.
 
**Setting up users**
After the final step in adding a user extension, you will see the following setup options to onboard the user.
• Send invite: Set up a user by sending a welcome email with an activation link.
• Activate by assigning credentials: Set up and activate a user by giving credentials. No welcome email will be sent.
• Activate later: Set up a user now but activate at a later time. No welcome email or notifications will be sent.
**Sending an invite to a user**
1. Select Send Invite under Setup Option.
2. Click on Edit Role under Assigned Role if you want to change the permissions of the user.
3. Click Next. The Add Users - Confirm window appears.
4. Review the charges and check the acknowledgment box at the bottom.
5. Click Next.
**Activating by assigning credentials to a user**
1. Select Activate by assigning credentials under Setup Option.
2. Fill in the info under Credential:
• Password
• Reenter Password
• PIN
• Reenter PIN
• Security Question
• Answer
3. Check the box for Temporary Password to prompt users to reset the password when they sign in for the first time (optional).
4. Under Emergency Address, click Add beside the name of users with devices.
5. Fill in the info for the emergency address. Click Done.
6. Click on Edit Role under Assigned Role if you want to change the permissions of the user.
7. Click Next. If you click Next without doing Steps 4-5, there will be a prompt for Missing Emergency Address. You may click Back to Add Emergency Address or Yes to continue without an emergency address. If you don’t add an emergency address at this point, the user(s) will be required to add their emergency address when they log in to their RingCentral online account or RingCentral app.
8. Review the charges and check the acknowledgment box at the bottom.
9. Click Next.
**Activating user at a later time**
1. Select Activate later under Setup Option.
2. Click on Edit Role under Assigned Role if you want to change the permissions of the user.
3. Click Next. The Add Users - Confirm window appears.
4. Review the charges and check the acknowledgment box at the bottom.
5. Click Next.
**Getting the details for Manual Provisioning** 
1. In the Admin portal, navigate to Phone System > Phones & Devices > User Phones.
2. Click on the name of the user you want to assign the Yealink phone.
3. Click Setup & Provision. 
4. Select the Other Phones tab, then click Select.
5. Select your desired Outbound Proxy from the dropdown menu, then click Copy the upper right corner to paste the provisioning details into a notepad.
**Provisioning Yealink phones manually**
To manually provision your Yealink device, you need a computer with access to the same subnet where your Yealink phone is running. You can be physically on-site, or you can use a VPN tunnel, remote connection, etc.
1. Get your Yealink phone’s IP Address.
2. Open a web browser and enter the phone’s IP address in the Address bar. 
3. Log in to the phone’s Web UI. The default username is admin, and the default password is admin.
4. Navigate to Account > Register.
5. Get the provisioning details and input the information to the following fields:
a. Line Active: Set to Enabled.
b. Label: Set the name to how you want to identify the line.
c. Display Name: Set the name to how you want to identify the line.
d. Register Name: Input the Authorization ID from the provisioning details.
e. User Name: Input the User name from the provisioning details.
f. Password: Input the Password from the provisioning details.
g. Sip Server 1 – Server Host: Input the SIP Domain, putting the URL into the first box and the port into the 2nd box.
h. Transport: If secure voice transport is set to Yes in the provisioning details, set to TLS. If it is set to No, set to TCP or UDP.
i. Enable Outbound Proxy Server: Set to Enabled.
j. Outbound Proxy Server 1: Input the Outbound Proxy, putting the URL into the first box and the port into the 2nd box.
6. Click Confirm.
The page should refresh. The Register Status should say “Registering” then switch to “Registered” after a few seconds.
Access your deskphone’s web interface
