---
title: Troubleshooting MAX Agent freezing
layout: layout-page-sidenav
description: When MAX agent freezes, there could be a few causes: attempting to change statuses, inability to click the submenus in the application and so forth. This means when customers call in, they may encounter an endless wait time because the agent has lost the call. The customer has to end the call for the entire interaction. To troubleshoot some of these issues, consider the following scenarios.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Troubleshooting MAX Agent freezing
redirect_from:
    - https://support.ringcentral.com/article-v2/Troubleshooting-MAX-Agent-freezing.html?brand=RingCentral&product=CC&language=en_US
---

### Troubleshooting MAX Agent freezing

When MAX agent freezes, there could be a few causes: attempting to change statuses, inability to click the submenus in the application and so forth. This means when customers call in, they may encounter an endless wait time because the agent has lost the call. The customer has to end the call for the entire interaction. To troubleshoot some of these issues, consider the following scenarios.
**Agent application freezes after agent dispositions the call**
**Issue:**
When attempting to disposition a call from a specific skill, the disposition menu may show a blank screen, or the agent console may completely freeze, locking the agent out. It generally results in the agent having to be force disconnected in Central and re-launching their agent console to return to an available state
**Resolution:**
Note: This workaround is specific to skills with required dispositions. Other factors can cause the agent console to freeze, which this solution will not resolve.
Navigate to Central > Manage > Skills > Post Contact.
On the Post Contact Tab, untick the Required box under the Disposition section.
Select the correct State to put the user in after the call.
Enter a max time limit to allow the agents to disposition in seconds.
Save your new skill settings.
Have agents assigned to this skill sign out and back into the agent console.
**Agent unable to change states in application**
**Issue:**
Agent application will randomly freeze or become unresponsive
User is consistently unable to change states or logout (chronic issue)
**Resolution:**
Data conflicts from the browser cache and cookies, Flash, and Java cache, and network connectivity issues. You can do the following to avoid and/or resolve the issues.
Confirm if the agent application is frozen or if only some portions are not responding.
If only some of the agent pieces are stuck, note which ones you cannot complete and report this to RingCentral support.
This can be done by attempting to do other actions in the agent, such as submitting agent feedback or looking at the Information pane.
If you can use other functions of the agent application, it is not frozen but is stuck in a specific process.
If you are not experiencing a chronic issue, force log out the agent.
Confirm internet connectivity by checking a third-party website or performing a ping test on the RingCentral Contact Center platform.
Clear cache and cookies from all web browsers.
Clear Flash cache. Ensure that all internet browsers are closed when doing this. This step is not applicable for MAX.
Clear Java cache. This step is not applicable for MAX.
Delete all items in the user's temp folder on their computer.
Ensure the user's default browser is set the same as everyone who has a working agent application.
Add RingCentral Contact Center sites as trusted sites in the browser.
If following the above procedures does not resolve the issue, contact RingCentral support and provide the following information:
The version of agent affected (MAX or Salesforce)
Specify if all or portions of Agent is frozen
Results of the RingCentral Contact Center ping test
Browser Developer logs (optional, but may be required)
**Agent application is freezing and not delivering emails or voicemails**
**Issue:**
Agent Application is:
Freezing
Not delivering emails
Not delivering voicemails
Other windows around agent Interface are freezing.
**Resolution:**
**For Windows**
Open your Windows Control Panel.
Search for Java In the upper-right search box.
Click the Java link to open the Java Control Panel.
Click the Security tab.
Click Edit Site List.
Click Add.
In the field that appears up top, enter: https://login.incontact.com/
Click OK. You should now see the URL in the Exception Site List section.
Click OK to close the Java Control Panel.

You may need to close your browser entirely and then re-open it so that the new Java settings are applied.
**For MacOS**
Click on the apple at top left and select System Preferences.
Click on Java
From there, follow steps 4-9 from the Windows instructions above. If you do not find Java in the System Preferences menu, you can search for it by opening up Finder and typing in /Library/Internet Plug-Ins/.
**Agent applications freeze after the agent dispositions the call**
**Issue:**
When attempting to disposition a call from a specific skill, the disposition menu may show blank or the agent console may completely freeze, locking the agent out. This generally results in the agent having to be force disconnected in Central and re-launching their agent console in order to return to an available state.
**Resolution:**
inContact Technical Support has identified a workaround for this issue.
Navigate to Central > Manage > Skills > Post Contact.
On the Post Contact tab uncheck the Required box under the Disposition section.
Select the correct State to put the user in after the call.
Enter a maximum time limit to allow the agents to disposition in seconds.
Click Save.
Have agents assigned to this skill, sign out and back into the agent console.
