---
title: Historical dashboards: Agent Disposition
layout: layout-page-sidenav
description: The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Historical dashboards: Agent Disposition
redirect_from:
    - https://support.ringcentral.com/article-v2/Historical-dashboards-Agent-Disposition.html?brand=RingCentral&product=EV&language=en_US
---


### Historical dashboards: Agent Disposition

The Engage platform provides several dashboards organized by categories that provide data on current information. Most of the reports used in dashboards can be found in the Standard folder of Historical reports.
Note: Dashboards and reports that reference digital data are reserved for future use.
Some parts of the UI will refer to reports as ‘insights.’ Reports are ‘insights’ as well. Still, most of the UI will only refer to reports as ‘reports’ and not ‘insights.’ Insight is a deprecated term.
The Agent Dispositions dashboard provides statistics of agent dispositions sliced by Product Group, Product, and Agent.

**Filters**
Date Range: A range of days that the dashboard will be covering. Preset to the last 30 days.
Account ID: The ID of the account that needs to be viewed.
Account: The sub-account to be reported on.
Channel Type: Narrows the report down to a certain channel type or a subset of channel types.
Product Type: Narrows the report down to a specific product type.
Product: Narrows the report down to a specific product/subset of products.
Agent Group: Narrows the report down to a subset of agent groups.
Agent Group ID: Narrows the report down to a subset of agent groups, using agent group IDs.
Agent Team: Narrows the report down to a subset of agent teams.
Agent Location: Narrows the report down to a subset of agent locations.
Agent Full Name: Narrows the report down to a subset of agents.
Agent ID: Narrows the report down using agent IDs.
Note: An activity is attributed to a time interval by its start timestamp. The account filter is a parent filter to the other filters (except for the Date). For example, if you select a particular account, the Agent Group filter will be showing only agent groups of that account.

**Agent Disposition Chart**
This bar chart shows the percentage of dispositions by product type, stacked to 100%. This means every product will show the percentage (x-axis) of dispositions of the product (y-axis).
Pending Disposition Time per Agent
Bar chart that shows the average time between when a call ends and a disposition is placed by each agent.
Agents without Agent Disposition
Shows the name of the agent as well as the number of interactions without dispositions.

**Agent Disposition Report**
This table shows the details of all agent dispositions.
Product group: Shows inbound queue groups and dial groups.
Product: Shows the product name (voice queue or campaign) within their product group.
Agent Full Name: Full name of agent associated with the disposition.
Agent Disposition: Shows the type of disposition the agent made, as determined by the admin at the product level. Rollup is the total number of Calls and % associated with the agent.
Calls: Number of calls associated with the disposition.
%: Percentage of calls associated with the disposition, in relation to the Rollup.

**Agent Pending Disposition Time**
Stacked bar chart that shows call disposition distribution by product.
