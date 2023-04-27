---
title: Historical dashboards: Omnichannel Overview
layout: layout-page-sidenav
description: The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Historical dashboards: Omnichannel Overview
redirect_from:
    - https://support.ringcentral.com/article-v2/Historical-dashboards-Omnichannel-Overview.html?brand=RingCentral&product=EV&language=en_US
---


### Historical dashboards: Omnichannel Overview

The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
Note: Dashboards and reports that reference digital data are reserved for future use.
Some parts of the UI will refer to reports as ‘insights.’ Reports are ‘insights’ as well. Still, most of the UI will only refer to reports as ‘reports’ and not ‘insights.’ Insight is a deprecated term.
The Omnichannel Overview dashboard provides you with the metrics you have for voice and digital interactions.

**Filters**
Date Range: A range of days that the dashboard will be covering. Preset to the last 30 days.
Account ID: The ID of the account that needs to be viewed.
Account: The sub-account to be reported on.
Channel Type: Narrows the report down to a certain channel type or a subset of channel types.
Agent Group: Narrows the report down to a subset of agent groups.
Agent Group ID: Narrows the report down to a subset of agent groups, using agent group IDs.
Agent Team: Narrows the report down to a subset of agent teams.
Agent Location: Narrows the report down to a subset of agent locations.
Agent Full Name: Narrows the report down to a subset of agents.
Agent ID: Displays by agent ID number.
Note: An activity is attributed to a time interval by its start timestamp. The account filter is a parent filter to the other filters (except for the Date). For example, if you select a particular account, the Agent Group filter will be showing only agent groups of that account.

**KPIs section**
This section shows the KPIs for the Omnichannel Overview. You will find the following metrics under this section:
Interactions: Total number of interactions incoming to a contact center for the selected period of time. Shows a comparison with the same count of interactions for the previous time interval of the same length. The change (shown in %) is displayed in green for an increased value and in red for a decreased value.
Interactions Handled %: Total number of interactions connected to agents during the selected period of time. Shows a comparison with the same count of interactions for the previous time interval of the same length. The change (shown in %) is displayed in green for an increased value and in red for a decreased value.
Agents Handling Interactions: Total number of agents that were working with interactions during the selected period of time. Shows a comparison with the same count of interactions for the previous time interval of the same length. The change (shown in %) is displayed in green for an increased value and in red for a decreased value.
Avg Handle Time: Average Handle Time over the interactions that were handled by Agents, with the condition that 'Agent Connected' = Yes. The change (shown in %) is displayed in red for an increased value, and in green for a decreased value. Note that Handle Time is calculated as a sum of Talk Time (which includes Hold Time) and Wrap Time.
Avg Queue Time: Average Queue Time over the segments that went through queues (filtered by Product Type values). The change (shown in %) is displayed in red for an increased value and in green for a decreased value.
Agent Voice Occupancy: Percentage of time that agents (shown on the KPI) spent engaged with voice interactions divided by the sum of time that agents were engaged with voice interactions with the time that agents were available to handle voice interactions. The change (shown in %) is displayed in green for an increased value, and in red for a decreased value. This metric is based on the Agent State dataset, where voice and digital states are reported separately, resulting in two separate metrics.
Agent Digital Occupancy: Percentage of time that agents (shown on the KPI) spent engaged with digital interactions divided by the sum of time that agents were engaged with digital interactions with the time that agents were available to handle digital interactions. The change (shown in %) is displayed in green for an increased value, and in red for a decreased value. This metric is based on the Agent State dataset, where voice and digital states are reported separately, resulting in two separate metrics.

**Distributions by Channel Type section**
You’ll find the following reports in this section:
Interactions: A bar chart showing interactions distributed by channel type.
Agents Handling Interactions: A bar chart that shows the number of agents handling interactions of a certain channel type within the selected period of time. Note that the values for this bar chart are not summed up in the Agents Handling Interactions KPI. Individual agents may handle multiple channel types.
Avg Handle Time: A bar chart showing how the average handle time differs between channel types. The difference between the Avg Handle Time in channel types and in KPI is that KPI averages all channel types. Having more than one channel type will impact the Avg Handle Time KPI.
Interactions by Channel Type by Agent: Table that shows the agent’s name and ID associated with the number of interactions by channel type (ex. Email, SMS, voice).

**Trends by Channel Type section**
You’ll find the following reports in this section:
Interactions: Shows a bar graph of the daily trend of the Interactions KPI by channel types. Clicking on a bar will show data down to the hour trend, showing how the handled interactions metric for a given channel type is distributed by the hour for that day.
Agents Handling Interactions: Shows a line graph of the daily trend of the Agents Handling Interactions KPI for each channel type separately. Clicking on the graph will display data down to the hour trend, showing how the same metric is distributed by the hour for that day.
Avg Handle Time (sec): A line chart showing a daily trend of the Avg Handle Time KPI for each channel type. Clicking on the chart will display data down to the hour trend, showing how the same metric is distributed by the hour for that day.

**Capacity Trends section**
This section contains trends that might demonstrate a possible correlation between Avg Queue Time and Agent Occupancy. For example, if Avg Queue Time increases while Agent Occupancy also increases or remains at an already high value, it might indicate high understaffing.
Under the Distributions by Channel Type section, you will find the following reports:
Avg Queue Time (sec) by Channel Type: Shows a line chart of the Avg Queue Time Handling Interactions KPI’s daily trend for each channel type. Clicking on the chart will display data down to the hour trend, showing how the same metric is distributed by the hour for that day.
Agent Occupancy Trend by Channel Type: Shows a line chart of Agent Voice Occupancy KPI and the Agent Digital Occupancy KPI’s daily trend. Clicking on the chart will display data down to the hour trend, showing how the same metric is distributed by the hour for that day. This metric is based on the Agent State dataset, where voice and digital states are reported separately, resulting in two separate metrics.

**Handle Time section**
This section contains the following reports:
Agent Avg Handle Time Distribution: Chart that shows the distribution (in percentage) of the average handle time of agents. Click on a value to drill down to the Agent Avg Handle Time Distribution Details report.
Interaction Handle Time Distribution: Chart that aggregates the number of interactions based on handle time intervals in minutes. Click on a value to drill down to the Interaction Handle Time Distribution Details report.
