---
title: Historical dashboards: Inbound Overview
layout: layout-page-sidenav
description: The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Historical dashboards: Inbound Overview
redirect_from:
    - https://support.ringcentral.com/article-v2/Historical-dashboards-Inbound-Overview.html?brand=RingCentral&product=EV&language=en_US
---


### Historical dashboards: Inbound Overview

The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
Note: Dashboards and reports that reference digital data are reserved for future use.
Some parts of the UI will refer to reports as ‘insights.’ Reports are ‘insights’ as well. Still, most of the UI will only refer to reports as ‘reports’ and not ‘insights.’ Insight is a deprecated term.
The Inbound Overview dashboard provides an overview of major inbound metrics and trends, helping contact centers analyze inbound activities and overall performance.
Inbound segments are those that are passing through queues from both voice and digital interactions. For voice interactions, product type is recorded in Voice Queue, while in digital interactions, product type is recorded in Digital Queue.

**Filters**
Date Range: A range of days that the dashboard will be covering. Preset to the last 30 days.
Account ID: The ID of the account that needs to be viewed.
Account: The sub-account to be reported on.
Channel Type: Narrows the report down to a certain channel type or a subset of channel types.
Product Group Type: Narrows the report down to product group types.
Product Group: Narrowing the report down to a specific product/subset of product groups.
Product Type: Narrows the report down to a specific product type.
Product: Narrows the report down to a specific product/subset of products.
Note: An activity is attributed to a time interval by its start timestamp. The account filter is a parent filter to the other filters (except for the Date). For example, if you select a particular account, the Agent Group filter will be showing only agent groups of that account.

**Inbound KPIs section**
This section shows the KPIs for the Inbound Overview dashboard. You will find the following metrics under this section:
Interactions: Shows the change in the number of interactions.
Queue Segments: This KPI shows the Queue Segment Count metric, which is how many times interactions were queued during the selected date interval.
Avg Queue Time: Shows the average queue time of segments that went through queues during the selected date interval, as filtered by product type values). The change (shown in %) is displayed in red for an increased value and in green for a decreased value.
Avg Queue Handle Time: Shows the average handle time over the queued segments that agents handled, with a condition that 'Agent Connected' = Yes. The change (shown in %) is displayed in red for an increased value and green for a decreased value. Note that Handle Time is calculated as the sum of Talk Time (which includes Hold Time), and Wrap Time.
Service Level %: Percentage of calls that passed SLA out of total calls queued.
Abandon Rate %: Percentage of calls abandoned.
RNA Rate %: Number of interactions that ring at an agent’s phone, but are not answered by the agent (Ring No Answer), as a percentage of all interactions assigned to that agent.
Repeated interaction: Shows the number of inbound interactions initiated by the same customer.

**Inbound Queues section**
This section drills into charts to see inbound queues distribution by Channel Type. Below are the metrics in this section:
Queue Segments: A chart showing the number of calls Accepted, RNA, Abandoned Deflected, and Agent Rejected.
Queue Segments Time: A bar chart showing how much time an inbound segment spends in different states during its lifetime: queue time, ring time, talk time, and wrap time. Clicking on a bar will show a pie chart, showing how the total time of a given segment state is distributed between channel types. For example, how total talk time is split between channel types.
Avg Queue Time by Channel Type: A bar chart showing how average queue time differs between channel types. Remember that value is averaged and not a summation. The Avg Queue Time KPI on the top is calculated from all inbound interactions; thus the average queue time for the channel types having more interactions will have more impact on the overall average handle time.
Avg Speed of Answer by Queue: Bar chart showing the average speed of answer in seconds by queues.
Acceptance Rate by Queue: Bar chart showing the acceptance rate in percentage by queues.

**Inbound Interactions, SLA Trends and Handle Time**
This section drills into charts to see Interactions distribution by Channel Type in the Inbound Interactions report.
Inbound Interactions: A stacked bar chart showing the number of times a call was queued.
SLA: Line chart that shows the percentage of calls or interactions that passed the SLA out of the total interactions queued.
Repeated Contacts Distribution: Shows the number of repeated contact distribution among buckets of unique contacts made by inbound interactions handled by an agent.
Handle Tiime and Repeated Customers: Shows the correlation between the average handle time spent by agents to solve customer problems and the number of repeat customers who made incoming interactions.
Interaction Handle Time Distribution: Chart that aggregates the number of interactions based on handle time intervals in minutes. Click to drill down to the Interaction Handle Time Distribution Details report.

**Inbound Queue Details section**
Contains the Inbound Overview report, a table that shows inbound details for their respective channels, queues, and queue groups.
This section allows you to export the report. Hover on the table and click on the More icon on its upper right. You can export the report into downloadable XLVL or CSV files. You can also click on Explore from here to download agent activity details with different metrics.
Below are the metrics covered in the entire Inbound Overview dashboard:
Interactions: A Queue Segment Count metric, which is the number of times interactions were queued during the selected date range. Click on a metric to drill down and access the Interaction Details report. Learn more about different metrics here.
Deflected: The number of calls sent to another destination.
Acceptance Rate: Percentage of interactions accepted by the agent over all the interactions handled.
Agent Rejected %: Percentage of interactions rejected by the agent over all of the interactions handled.
RNA %: Percentage of interactions that ring at an agent’s phone, but are not answered by the agent (Ring No Answer), as a percentage of all interactions assigned to that agent.
Abandon Rate %: Percentage of interactions abandoned.
Short Abandon %: Interactions abandoned after a short time of waiting.
Manual Dials Rate: Percentage of manually placed calls over all calls.
Manual Dials No Connect Rate: The percentage of manually placed calls by an agent, but not connected.
External Transfer Rate %: Percentage of inbound segments being externally transferred from queues as a ratio to all inbound segments placed in queues.
Avg Queue Time: The total time spent waiting in queue.
Avg Queue Handle Time: Average time it took an agent to handle an interaction that arrived through a queue.
Avg Queue Abandon Time: The average time a customer waited in a queue before dropping the interaction.
Avg Speed of Answer: Average time the caller waited to be connected to an agent through the entire interaction. If sliced by queue, will show how much time on average callers wait in the particular queue for the call to be answered.
Avg Talk Time: The average time a customer spent on the phone connected to an agent or IVR (including time on hold).
Avg Wrap Time: The average time an agent spent after a customer disconnected before submitting call disposition.
Avg Handle Time: The Average Handle Time over the interactions that were handled.
SLA Passed: The number of calls answered within configured service level threshold.
Service Level: Percentage of calls that were connected to an agent within configured SLA out of total calls queued.
