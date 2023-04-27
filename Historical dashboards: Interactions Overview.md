---
title: Historical dashboards: Interactions Overview
layout: layout-page-sidenav
description: The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Historical dashboards: Interactions Overview
redirect_from:
    - https://support.ringcentral.com/article-v2/Historical-dashboards-Interactions-Overview.html?brand=RingCentral&product=EV&language=en_US
---


### Historical dashboards: Interactions Overview

The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
Note: Dashboards and reports that reference digital data are reserved for future use.
Some parts of the UI will refer to reports as ‘insights.’ Reports are ‘insights’ as well. Still, most of the UI will only refer to reports as ‘reports’ and not ‘insights.’ Insight is a deprecated term.
The Interactions Overview dashboard provides an overview of all contact center interactions with their respective metrics and details.

**Filters**
Date Range: A range of days that the dashboard will be covering. Preset to the last 90 days.
Account ID: The account ID that needs to be viewed.
Account: The account to be reported on.
Channel Type: Narrows the report to a specific channel type or a subset of channel types.
Product Group Type: Narrows reports to product groups (ex. Dial Group, IVR Group, etc.).
Product Group: Shows products by group name.
Product: Displays product name.
Agent Full Name: Narrows the report to a subset of agents.
Agent ID: Displays by agent ID number.
Agent Group: Narrows the report to a subset of agent groups.
Agent Group ID: Displays by agent group ID number.
Agent Team: Displays agent teams.
Agent Location: Displays by agent location.
ANI: Displays by ANI (Automatic Number Identification).
DNIS: Displays by DNIS (Dialed Number Identification Service).
UII Date: Displays the attribute for the date part of the UII (YYYYMMDD).
UII Time: Attribute for the time part of the UII (HHMMSS).
UID: Attribute for the last 16 digits of the UII (013VRU00000XXXXX).
Note: An activity is attributed to a time interval by its start timestamp. The account filter is a parent filter to the other filters (except for the Date). For example, if you select a particular account, the Agent Group filter will show only the agent groups of that account.

**Interactions KPIs section**
This section shows major interactions related to KPIs. You will find the following metrics under this section:
Interactions: Total number of interactions incoming to a contact center for the selected time. Shows a comparison with the same count of interactions for the previous time interval of the same length. The change (shown in %) is displayed in green for an increased value and in red for a decreased value.
Segments: Shows the total number of segments for all incoming interactions to a contact center for the selected time period.
Avg Handle Time: Average time it took the agent to handle the call.
Avg Talk Time: Average time customers spend on the phone connected to an agent or IVR per interaction segment.
Avg Hold Time: Average time the customer was put on hold by the agent during the interaction.
Avg Wrap Time: Average time it takes the agent to submit a disposition after the interaction is disconnected.

**Interactions Trend and Distribution section**
This section contains reports that show weekly and monthly interaction trends and their distribution by channel type and call type.

**Interactions Handled by Channel Type**
Pie chart that shows the number of interactions handled by channel type.

**Interactions by Call Type**
Shows a monthly trend of inbound and outbound interactions. Click a data point to drill down daily interaction trends.

**Talk Time & Interactions**
Shows a weekly trend of interactions and their overall talk time. Click a data point to drill down daily interactions and talk time trends.

**Interaction Handle Time Distribution**
Chart that aggregates the number of interactions based on handle time intervals in minutes. Click a data point to drill into the Interaction Handle Time Distribution Details report.

**Weekly Interactions Trend**
Shows a weekly trend of incoming interactions. Click a data point to drill down daily interaction trends of a reported week.

**Monthly Interactions Trend**
Shows a monthly trend of all incoming interactions. Click a data point to drill down daily interaction trends of a reported month.

**Interaction Details section**
**Interaction Details**
Table that shows the details of interactions. This report contains the following interaction-related attributes and metrics:
UII: Displays a unique identifier for an interaction. Learn more about UII.
Segment Index: Number of segments of an interaction.
Date (Started): Start day of the interaction.
Call Started Time: Timestamp when a call is started.
Channel Type: Channel type (voice or digital interaction) of an interaction.
Call Type: Inbound or outbound.
Dial Type: Type of outbound calling.
ANI: Displays the interaction's automatic number identification (ANI).
DNIS: Displays the interaction's dialed number identification service (DNIS).
Product Type: Displays products by type.
Product: Displays product name.
Agent Full Name: Displays agents by their full name.
Agent Team: Displays agent teams.
Call Result: Different call results, such as inbound abandon or inbound defected, among many others.
Termination Reason: Reason a call was terminated.
Agent Disposition: Type of agent disposition data to display — default, requeue, or to not display at all.
Abandon Type: Displays long or short type of call abandons.
SLA Qualified: Presents data that passed SLAs. The SLA calculation won’t count short calls.
SLA Passed: Shows calls that were answered by the agent within the threshold configured for the queue.
Recording URL: Provides the URL for phone call recordings.
RNA: Number of calls ringing at agent phone, but not answered by the agent (Ring No Answer).
Queue Time: Total time spent waiting in the queue.
Ring Time: Ring time duration.
Outbound Ring Time: Total ringing time for outbound calls.
Handle Time: Total time spent handling interactions.
Talk Time: Time the customer spends on the phone connected to an agent or IVR (time on hold included).
Wrap Time: Time the agent spends after the customer disconnects before submitting call disposition.
