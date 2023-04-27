---
title: Historical dashboards: Agent Activity
layout: layout-page-sidenav
description: The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Historical dashboards: Agent Activity
redirect_from:
    - https://support.ringcentral.com/article-v2/Historical-dashboards--Agent-Activity.html?brand=RingCentral&product=EV&language=en_US
---


### Historical dashboards: Agent Activity

The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
Note: Dashboards and reports that reference digital data are reserved for future use.
Some parts of the UI will refer to reports as ‘insights.’ Reports are ‘insights’ as well. Still, most of the UI will only refer to reports as ‘reports’ and not ‘insights.’ Insight is a deprecated term.
The Agent Activity Dashboard provides an overview of voice and digital agent activity. This dashboard has metrics that are split by channels. In the current release, the agent state data feed doesn't provide states on a channel level but provides voice and digital states separately, so the metrics built on the agent state feed can only be sliced by voice or digital data. Also, metrics that are built on segment feed can be sliced by channels where needed.

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
Agent Disposition: Filters by agent disposition.
Note: An activity is attributed to a time interval by its start timestamp. The account filter is a parent filter to the other filters (except for the Date). For example, if you select a particular account, the Agent Group filter will be showing only agent groups of that account.

**Agent KPIs section**
This section shows major agent KPIs. Below are the metrics under Agent KPIs sections:
Agents: Total number of agents that were logged in. Shows a comparison with the same count of agents for the previous time interval of the same length. The change (shown in %) is displayed in green for an increased value and in red for a decreased value.
Voice Login Utilization: Percentage of an agent’s login time spent handling voice customer interactions. The change (shown in %) is displayed green for an increased value and in red for a decreased value.
Agent Voice Occupancy: Time an agent is engaged in productive work as a percentage of the time they are available to do productive work for voice interactions.
Digital Login Time Utilization: Percentage of an agent's login time spent handling digital customer interactions. The change (shown in %) is displayed green for an increased value and in red for a decreased value.
Agent Digital Occupancy: Time an agent is engaged in productive work as a percentage of the time they are available to do productive work for digital interactions.
Interactions: Total number of interactions that come into the platform.
Interactions Assigned: Number of interactions assigned to an agent. Shows a comparison with the same count for the previous time interval of the same length. The change (shown in %) is displayed green for an increased value and in red for a decreased value.
Interactions Handled: Number of interactions an agent was able to handle. Shows a comparison with the same count for the previous time interval of the same length. The change (shown in %) is displayed green for an increased value and in red for a decreased value.
RNA Rate: Number of interactions that rang the agent's phone but were not answered (Ring No Answer) as a percentage of all interactions assigned to that agent.
Avg Handle Time: Average time it takes an agent to handle an interaction that is assigned to him. Includes Wrap Time. The change (shown in %) is displayed in red for an increased value and in green for a decreased value.

**Trends section**
This section shows charts on interactions and agent time distribution by channel type. Below are the reports for the Trends section:
Agents and Handled Interactions: Shows the Agents and Interactions Handled KPIs by day. Clicking on a bar will drill down to a pie chart, showing the number of interactions per channel for that day.
Agent Ring, Talk and Wrap Time: Stacked bar chart showing the daily total of ring, talk, hold, and wrap time of segments handled by agents. Clicking on the bars of the chart will show how time is distributed by channels.
Agents Monthly Trend: Line chart showing logged-in agents per month, for the specified time period or year.

**Agent Login and Interaction Time Distribution section**
This section shows charts with the agent’s login time distribution breakdown by channel type within a specific product. Below are the metrics under Agent Login and Interaction Time Distribution section:
Voice Login Time: Stacked chart based on metrics that are built on the agent base state feed. Shows how agents login time was distributed between engaged time (Engaged base states), available time (Available base state), and other times (a combination of all other base states). This bar chart is an extension of the Voice Agent Login Utilization KPI, which is displayed here as Voice Engaged Time %.
Digital Login Time: Stacked chart based on metrics that are built on the agent base state feed. Shows the percentage of digital working (Chat-engaged digital state), available (Chat-available), and other (a combination of all other digital states) states the time of the total agent’s login time. This is an extension of the Digital Agent Login Utilization KPI, which is displayed here as Digital Engaged Time %.
Agent Interaction Time by Channel Type: Stacked bar chart based on metrics built on the interaction segment feed. It shows the distribution of Ring Time, Talk Time, and Wrap Time breakdown by product type. Percentages here are rounded. Note that talk time includes hold time.

**Agent Activity Details section**
This section shows more charts that are helpful in getting a rounded overview of agent activities.
Agent Handle Time Analysis
Bubble chart that shows the correlation between Avg Talk Time (x-axis) and Avg Wrap Time (y-axis), taking into account the interaction volume (segments in measure, bubble size) by agent (view by).
Each bubble represents an agent, while the bubble size represents the total number of call segments. The x-axis represents the average talk time (in seconds), or the average time the customer spent on the phone connected to an agent. The y-axis represents average wrap time (in seconds), or the time the agent spends submitting the call disposition after the call ends. It shows the correlation between Avg Talk Time and Avg Wrap Time, taking into account the Interaction volume handled by the Agent. This helps contact center management analyze Agent performance and conduct.
Voice Agent Utilization & Occupancy Trend
This line chart compares Voice Agent Utilization vs Voice Agent Occupancy over time.

**Agent Activity Report**
Shows statistics for agent activity, broken down by Agent Group and by individual Agent.
This section allows you to export the report. Hover on the table and click on the More icon on its upper right. You can export the report into downloadable XLVL or CSV files. The report in the table format shows statistics broken down by Agent Group, and by individual Agent.
The following metrics below cover the entire agent activity dashboard:
Agent Group: The agent group of the agent whose stats are displayed.
Agent Full Name: Full name of the agent whose stats are displayed.
Agent ID: Identification number of the agent whose states are displayed.
Assigned: Number of assigned interactions.
Agent Connected %: Rate of interactions connecting to an agent.
RNA %: Rate of ring no answer (RNA).
Manual Dial Rate: Rate of manual dials for all interactions of an agent.
Manual Dial No Connect Rate: Rate of manual dials that did not connect of an agent.
Avg Handle Time: Average Handle Time over the interactions that were handled by agents.
Avg Ring Time: The average ring time over the interactions that were ringing at agents.
Avg Talk Time: The average talk time over the interactions that were handled by agents.
Avg Hold Time: The average time an agent puts a call on hold.
Avg Wrap Time: The average time an agent spent after a customer disconnected before submitting call disposition.
Login Time: Total agent login time.
Voice Agent Login Utilization: The percentage of an agent’s login time spent handling voice customer interactions.
Voice Agent Occupancy Rate: The percentage of the time that an agent is available to do productive work relating to voice interactions.
Digital Agent Login Utilization: The percentage of an agent’s login time spent handling digital customer interactions.
Digital Agent Occupancy Rate: The percentage of the time that an agent is available to do productive work relating to digital interactions.
Interactions by Channel Type by Agent
Table that shows the agent’s name and ID associated with the number of interactions by channel type (ex. Email, SMS, voice).
