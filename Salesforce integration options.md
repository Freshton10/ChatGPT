---
title: Salesforce integration options
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Salesforce integration options
redirect_from:
    - https://support.ringcentral.com/article-v2/assisted-provisioning-yealink-deskphones.html?brand=RC_US&product=RingCentral_MVP&language=en_US
---

### Salesforce integration options

**Salesforce Agent Adapter**
Agent Adapter for Salesforce is an agent interface that contains many of the same features and functionality found in MAX. Agent Adapter integrates directly into Salesforce so you don’t have to jump between the two agent applications.
**Features**
Perform default and custom screen popouts on any Salesforce object and any contact channel.
Default query / screen popout: Agent for Salesforce takes the ANI (Automatic Number Identification) of the caller, passes it into Salesforce, and Salesforce performs a query for the ANI and pops an object based on the settings set forth in the softphone layout in Salesforce.
Custom query / screen popout: Salesforce queries are driven by caller IVR input, script calculations, external database queries, and Salesforce queries from within the IVR script. This includes Visualforce pages and the ability to pass information as a variable to the Visualforce page.
Automatic creation of task and activity records in Salesforce that can include any information about the call.
Click-to-dial from within Salesforce.
Support for both the Classic View and Lightning Experience. You can learn about switching between interfaces, enabling Lightning Experience, and more at https://help.salesforce.com.
**Login interface**

Agent Name - Enter the username.
Agent Password - Enter the password.
Phone Number - Select if you will be using a number.
Station ID - Select if you will be using a Station ID.
Agent Phone - If you selected Phone Number, enter the digits.
Enable Automatic Login - Select to automatically login to the adapter upon login to Salesforce.
Enable Tooltips - Select to display specific information about each user interface icon when the mouse hovers over it.
Log Level - Elect from the dropdown the level to log into.
Save - Click to save the information selected above.
Option - Click to log out. It does not happen automatically when you close the application.
**Main interface**

Messages indicator: Indicates that there are one or more unread Agent Messages. If there are no unread messages, no numbers will be displayed.
Agent leg status: Displays your connectivity status.
Availability status: Shows your current state in the contact center. It provides a way for you to change your status. The time in state (shown below the Availability Status bar) restarts when the status changes.
Phone: Initiates an outbound call using the keypad. Your availability status doesn’t need to be set to Available to make an outbound call. You can click the numbers or use the keyboard to enter a number to dial.
Agents: Displays a list of other agents and their availability state. You can filter the list or search for a specific agent. Clicking an agent in the list initiates an outbound call to that agent.
Skill list: Displays a list of skills assigned to you, the number of contacts in the queue for that skill, and the longest wait time in each queue. You can filter the list or search for a specific skill. Clicking a skill in the list initiates handling a contact with that skill.
Address books: Displays your address books. All address books assigned to you are accessible here. You can search for an address book or use the drop-down to select one from a list. Clicking a contact in an address book displays that contact's details. You can click the mobile, email, or phone icon in the details to initiate a connection to that contact based on the icon you click.
Contact history: Displays your contact history. You can filter the list or search for a specific contact.  You can click a contact to display a skill selection list, and then select a skill to initiate an outbound call to the phone number in the contact history.
Information: Displays basic information about you (the agent), including the currently installed version of Salesforce and a list of skills assigned to your user account.
Email: Initiates the email feature. Your availability status does not need to be set to Available to create an email. Click the icon to access the email interface.
Commitment manager: Displays a list of pending commitments and the option to create a new commitment. Select Me to view your own commitments or Skill to view commitments assigned to a skill queue.
Agent reports: Displays the Agent Reports dashboards, which allow you to view your performance and productivity.
Agent messages: Displays agent messages.
Help: Redirects you to the Help site.
Options: Allows you to change personal information, submit feedback about Agent Adapter for Salesforce, download the Agent for Salesforce log, and log out.
Phone queue: Displays the number of contacts in all assigned phone skill queues.
Work item queue: Displays the number of contacts in all assigned work item skill queues.
Chat queue: Displays the number of contacts in all assigned chat skill queues.
Personal queue: Displays the number of contacts in your personal queue.
Email queue: Displays the number of contacts in all assigned email skill queues.
**NICE CXone Agent**
Agent for Salesforce integrates the NICE CXone Agent application into Salesforce. This allows you to handle interactions directly instead of jumping between applications. Your administrator can select one of the three user interfaces for you to use: Classic, Classic in Lightning, or fully integrated Lightning Experience.
**Lightning Agent**
The fully integrated Lightning Agent for Salesforce allows your organization to have agents handle many kinds of interactions. Depending on what your organization needs and been configured to support, you might handle some or all of these kinds of interactions:
Omnichannel interactions: Omnichannel interactions can be phone, email, and chat. These interactions appear on the Omni tab. Agent for Salesforce uses the skills your administrator assigns to you to determine what omnichannel interactions to send to your queue. You need to be assigned omnichannel skills to access interactions on the Omni tab.
Digital interactions: Digital interactions can be messaging from a variety of online platforms, including Facebook, Instagram, Twitter, and WhatsApp. Digital interactions can also be chat and email. These interactions appear on the Digital tab. Agent for Salesforce uses the digital routing queue your administrator assigns to you to determine what digital interactions to send to your queue. You need to be assigned routing queues to see the Digital tab.
Both omnichannel and digital interactions can include chat and email. Our organization will determine how it wants to handle chat and email interactions.
**Lightning interface**
Agent for Salesforce may display icons instead of text. You can hover over the icon to see the related text. This feature is managed by your administrator.

Popout: Allows the agent to pop out the contact into a bigger screen for handling.
Availability status:Shows the agent's state in the contact center. It provides the agent with a way to change the status. The time in state (shown below the Availability Status bar) restarts when the status changes.
Agent leg status: Displays the agent's connectivity status (connected, attempting to connect, not connected).
Omni: Displays omnichannel interactions, such as inbound or outbound calls, chat, and email. This tab is visible to all agents, even those who aren't configured to handle omnichannel interactions.
Schedule: If WEM is enabled, you can find the agent's WEM schedule and a list of commitments assigned to the agent. Click the WEM link at the bottom of the agent to pop out a window that displays additional information.
Alerts: Displays alerts related to the agent and their activity.
Settings: Allows the agent to view personal and platform information, log settings, online help, set A/V notifications, and agent reports and performance.
Address book: Displays the address books assigned to the agent. The agent can search for an address book or use the drop-down to select one from a list. Selecting a contact in an address book displays that contact's details. The agent can click the mobile, email, or phone icon in the details to initiate a connection to that contact based on the icon the agent clicks.
New: On the Omni tab, it allows the agent to initiate an outbound call, create a new commitment, or request a contact, if enabled.
On the Digital tab, it allows the agent to create an outbound email or chat, if enabled.
On both tabs, you must have the skill or be assigned to a routing queue that allows you to perform these actions.
Queue counter: Displays the number of contacts in the queue of the skills assigned to the agent. The queue counter only shows the counts of omnichannel interactions. If you only handle digital interactions, the counters will always show 0.
**Other options**
**Setting up Connected App and obtaining Consumer Key and Secret**
To set up the Connected App, log in to Salesforce. Go to Setup > Create > Apps. In the Connected Apps section at the bottom, click New. The following window will appear:

Complete the following setup in the highlighted fields.
Connected App Name - inContact Integration
API Name - inContact Integration
Contact Email - pssf@incontact.com
Put a checkmark in the box to enable OAuth Settings. (This will show the additional OAuth settings)
Enter Callback URL
Production Environment - https://login.salesforce.com/services/oauth2/callback
Test/Sandbox Environment - https://test.salesforce.com/services/oauth2/callback
In the Available OAuth Scopes section, a couple options will provide a certain level of access. If possible, the setup should be to allow Full Access. This will ensure no hiccups with permissions and data mapping going forward. If unwilling to provide this level of access, select “Access and manage your data (API)”. Note: Please make sure you are aware of any security concerns you may have if you choose to select Full Access.
Click Save.
The following window will appear that shows both the Consumer Key and the Consumer Secret, which will need to be provided to inContact:

We recommend Connected App Name and API Name follow the naming convention “inContact Integration”, but it is not required. We also suggest the contact email be named pssf@incontact.com. This is a shared mailbox used by the Expert Services team to monitor and set up specific integration points within Salesforce. This helps avoid any problems with passwords being reset and so forth.
