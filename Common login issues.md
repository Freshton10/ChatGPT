---
title: Common login issues
description: To help support Contact Center customers, we’ve listed below some common login issues, along with their resolutions.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Common login issues
redirect_from:
    - https://support.ringcentral.com/article-v2/Common-login-issues.html?brand=RingCentral&product=CC&language=en_US
---


### Common login issues

To help support Contact Center customers, we’ve listed below some common login issues, along with their resolutions.
MAX Agent login issues
Missing option to login to MAX using phone or station ID in Userhub
When logging in to MAX, you don’t see the option to log in via phone number, station ID, or integrated softphone.

These options are turned off under the Roles and Permissions. To turn them back on:
Log in to RingCentral Contact Center.
Select Admin > Roles and Permissions.
Select the security profile of the user whose connection option you wish to change (usually,  the company’s Agent profile).
Select the Permissions tab.
Click ACD> MAX (Agent Interface).
Toggle the following options on or off for the user:
Set Phone Number
Set Station ID
Integrated Softphone
Click Save

Error message: Unable to authenticate with the given credentials
Clicking Launch Agent opens the MAX window but generates this error message: “Unable to authenticate with the given credentials.”
Possible causes:
The agent launched the MAX agent application on an unsupported browser.
The agent’s date, time, or time zone settings are incorrect.
The user’s VPN, proxy server, or security software is blocking or limiting access to certain websites.
Resolutions:
Make sure the agent is using a supported web browser.
Make sure that the agent’s computer’s date, time, and time zone settings of the computer are correct.
Work with the agent to adjust the settings on any VPN, proxy server, or security software (e.g., Symantec WSS Agent) that they may be using. For testing and isolation, disconnect these services one at a time while the agent logs in. The agent may need to restart their computer for the changes to take effect.
Agent can’t access their integrated softphone
An agent can’t access their integrated softphone when they log in to MAX Agent.
Possible causes:
The agent is using an unsupported web browser.
The agent hasn’t selected Integrated SoftPhone and MAX upon logging in.
The Business Unit hasn’t been set up for MAX with an integrated softphone.
The integrated softphone hasn't been enabled in the agent’s security profile.
Resolutions:
Make sure the agent is using a supported web browser
In the Agent interface, the agent should select Integrated Softphone when they connect to inContact.
The agent’s security profile in Central or User Hub must permit access to the Agent software and integrated softphone.
Note: If none of these resolutions fixes the problem, contact your inContact representative.
Agent is repeatedly locked out of MAX and must reset password daily
If an agent is repeatedly locked out of MAX and has to reset their password daily, the cause likely has to do with an application that is trying to log in with the agent’s previous credentials. To fix the issue:
Log in to RingCentral Contact Center.
Click Admin > Users.
Search for the name of the user who’s having login issues.
In the General tab, add a single digit to the agent’s username.
Click Save, then try logging again.
Agent leg won’t connect to MAX
MAX Agent can’t connect to the user’s phone.
Possible causes:
Problems with the phone or phone number
Resolution:
Log in to Contact Center.
Click on ACD.
Select Stations.
Check the Audit Log / Login History to verify the dialed phone number.
Other options:
Test the call agent leg phone number with one or two methods:
Call it from a regular phone, or
If it’s a 700 or 999 number, call it from the agent application.
Have the agent log in using a different phone number, such as their mobile phone.
Make sure the station ID matches the phone number.
Make sure the station phone number includes no spaces or dashes.
If this process doesn’t resolve the issue, contact our Support Team. Make sure you have the following information ready:
The names of the agents who have this issue
A list of any error messages they’ve received
The relevant Agent leg numbers
A MAX client initialization error prevents agents from being available
If an agent, upon login, sees a Client initialization error  that prevents them from going Available, follow these tips to resolve the issue:
Close all browsers.
Clear all temp files from the browser.
If the agent is using the MAX agent with an integrated softphone, the initialization error could be caused by a headset issue. Try a different headset, and/or verify that the existing headset is compatible with and connected to the agent’s browser.
Note: Some users may be able to get past the error message after a few attempts, while others still encounter the error after optimizing the browser per the above instructions. Contact Tech Support if the issue persists.
SSO login issues
Error message: Could not authenticate when SSO tries to verify a user via email
An agent may receive the error message “Could not authenticate” when they try to verify their SSO via email.
Possible cause:
The email address in the agent’s identity provider may not exactly match their external identity value. 
Resolution:
To solve, the users have all lowercase domains and some have all uppercase. The uppercase ones need to be changed to lowercase. It isn't the email that matters, it is the External Identity.
Unable to authenticate via SAML 2 SSO in User Hub
A user may be unable to use SAML 2 SSO to authenticate.
Possible cause:
Periodic failure to synchronize user information can cause this issue.
Resolution:
Log in to RingCentral Contact Center.
Go to Admin.
Click Users and select the user.
Click Edit.
You can now change the role to one that uses an authenticator other than SAML. Then change the role back to its original definition. The agent will have to validate their email again to force synchronization.
Click Save.
Unable to log in using the Salesforce Agent SSO link
A duplicate agent was created and the original agent cannot log in using the SSO.
Possible cause:
If an agent does not go to Admin > My Account > Link Account, the Subject and Issue Field will be linked to the duplicated account and not the original account.
Resolution:
Create a technical support case for the duplicated user info (username) requesting the Issuer and Subject field's removal from the agent's profile in our database.
Unable to log in to an inContact-hosted FTP site
When attempting to login to an inContact hosted FTP site, a user receives the error Authentication failed. Critical error. Could not connect to the server. inContact will automatically disable the inContact Hosted FTP site after 90 days of inactivity. Resolution.
You will need to contact your Technical Account Manager or Technical Success Advisors to have your FTP site re-enabled.
Station ID login issues
Error message:  Station ID is not valid in MAX Agent
A user receives the error message Station ID is not valid when trying to log in.
Possible cause:
The user is trying to enter their phone number in the Set Station ID field instead of the Set Phone Number field.
Resolution:
Log in to RingCentral Contact Center.
Click Launch Agent > Set Phone Number.
Enter the phone number in the Phone Number field
Click Continue.
Configured station ID/phone number differs from the current station ID/phone
When an agent logs in to Salesforce Agent, they receive the following error message:Your configured station ID or phone number is different from the station ID/Phone number currently in use. Your configured station ID Phone number is: XXXXXXXXXXXX.
Possible cause:
The agent hasn’t correctly logged out of their Salesforce Agent session.
Resolution:
Log out of Salesforce agent. This will clear any previous station/phone number information.
Log into Salesforce Agent with the correct information.
Phone number or station ID is in use
When attempting to log in with the Set Phone Number option, an agent receives the error message Phone number or station ID is in use.

Possible cause:
Another agent is currently logged in with the same phone number.
Resolution:
Make sure the MAX user has permission to use the phone number to log in.
Log in to the Contact Center.
Click on Admin.
Underneath the security dropdown in the left side menu, click on Roles and Permissions.
Click the agent/s name in the Permissions list.
Click the Permissions tab.
Click on MAX. Assure the toggle switches are on.

Search the active agents report to locate the agent using the number.
Log in to the Contact Center.
In the left side menu, select Reporting.
Click on Active Agents in the Reports List.
Click Run Report.
The Active Agents report shows the number of agents who are actively connected to the system and their current activity at the moment you run the report. With this information, you will quickly be able to evaluate what your agents are doing. From this report, you can also log your agents out of the system and even clear stuck agents using the Terminate option.
Error: Concurrent agent limit or station limit exceeded
User receives the error message Concurrent agent limit or station limit exceeded when trying to enter station ID.

**Possible cause:**
The account may have reached its station limit.

**Resolution:**
Log in to RingCentral Contact Center.
In the main menu, click Reporting.
Select the Billing Report Station tab and see how much the customer is using.
You can also select the Business Unit Usage tab to check the account’s station limit
If the customer’s usage figure is above the limit set, the customer's account’s main contact must request a station-limit increase from their Technical Account Manager or Customer Service Team.
