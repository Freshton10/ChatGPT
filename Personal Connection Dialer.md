---
title: Personal Connection Dialer
description: Contact Center’s Personal Connection (PC) Dialer autodials numbers and tracks information about those calls. PC Dialer provides agents with progressive, proficient, and prioritized calling abilities.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Personal Connection Dialer
redirect_from:
    - https://support.ringcentral.com/article-v2/Personal-Connection-Dialer.html?brand=RingCentral&product=CC&language=en_US
---


### Personal Connection Dialer

**Navigating to the Personal Connection Dialer**
Log in to RingCentral Contact Center.
In the main menu on the left side, click ACD.
In the Outbound dropdown, select Skill Control.
**General settings**
To edit these options,  you can click on “Edit” in the Outbound Skills menu.
Details: ID, Media Type, Status, Name
Parameters: General retry call settings, frequency of calls.
Call Suppression: Enable scripts to handle call suppression.
Do Not Call (DNC): Lets you add numbers to Do Not Call lists and remove those numbers from the outbound dialer.
Tags: Add tags to calls to help with call tracking.
Additionally, the settings panel allots the ability for administrators to view notes from agents and see the audit history of all calls made with the dialer.
**Dialing modes**
Personal Connection supports multiple dialing modes (sometimes called dialing strategies), which you configure on a per-skill basis.
Predictive: Sometimes called overdialing. The dialer places from two to six calls at a time per agent. If your inContact representative has restricted your dialing to 1:1, you won’t be able to use this dialing mode.
Progressive: The dialer places one call at a time per agent.
Preview: The dialer requires the agent to choose predictive mode or progressive mode from a popup. The agent must accept or reject the call within a certain period of time before a default action occurs.
Agentless: The dialer places calls without an agent’s input. The dialer can leave messages, play information, or create a proactive IVR experience via Studio scripting.
Manual: The agent places calls manually. N The dialer uses no in-platform calling list or automated dialing features.
Non-telephony: An option for records or destinations that require compliance handling.
**Dispositions**
A disposition documents the result of a Personal Connection attempt by the system or the agent. Dispositions trigger other actions, including finalizing a record, retrying a record, scheduling a callback, and adding to a Do Not Call list. It is best practice to require agents to select a disposition for each call; however, it is technically possible to leave it blank,  but we do not recommend it, as no disposition could lead to misleading outcomes.
All calls handled by an agent without an agent selecting a disposition and/or classification will be finalized.
A classification must be assigned to the disposition to be used in a Personal Connection Skill.
Agent dispositions must be classified to be assigned to a Personal Connection skill, and to determine the next action for the call record. Depending on the classification selected for the agent disposition, the following information will automatically be populated:
Reporting Group: The grouping of related dispositions
System Outcome: The system’s applied outcome to the disposition record
Require Commitment Amount: Agent must enter the customer’s commitment figure/amount.
Require Reschedule Date: Agent must enter a date on which the dialer should call the contact again.
Agent Specific: Indicates the callback is assigned to the agent who scheduled it.
Agentless Skills require dispositions to be set up with a custom script in the set disposition action.
Note: System dispositions are placed in a record when the call is not passed to an agent and requires an outcome. These dispositions are used for no answer, busy, errors, and other related outcomes.
