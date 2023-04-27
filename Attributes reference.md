---
title: Attributes reference
layout: layout-page-sidenav
description: Attributes are non-measurable descriptors used to break down metrics and measures and represent qualitative data. Attributes can also be used as filters in your reports, KPI widgets, and dashboards.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Attributes reference
redirect_from:
    - https://support.ringcentral.com/article-v2/Attributes-reference.html?brand=RingCentral&product=EV&language=en_US
---


### Attributes reference

Attributes are non-measurable descriptors used to break down metrics and measures and represent qualitative data. Attributes can also be used as filters in your reports, KPI widgets, and dashboards.
Note: Attributes marked as ‘Digital’ you may see in the UI are for a future release.

**Agent**
Agent AHT Buckets: Time intervals or buckets showing agent average handling times. Time intervals are by 60 minutes. (00:00 to 00:59, 01:00 to 01:59, etc.)
Agent Email: Email registered when an agent is created.
Agent First Name: Displays agents by their first name.
Agent Full Name: Displays agents by their full name.
Agent Group: Displays agent groups by name.
Agent Group ID: Displays by agent group ID.
Agent ID: Displays by agent ID number.
Agent Last Name: Displays agents by their last name.
Agent Location: Displays agents by their location.
Agent Login ID: Displays agents by their login ID number.
Agent Team: Displays agent teams.
Agent Type: Distinguishes agents from supervisors.

**Agent State**
Agent First Login Time: First login time of an agent on a particular day.
Agent Last Logout Time: The timestamp of an agent’s logout time.
Agent Login End Time: The timestamp of an agent login session end.
Agent Login Start Time: The timestamp of an agent login session start.
Agent State End Time: The actual end time of an agent state (HH:MM:SS).
Agent State Start Time: The actual start time of an agent state (HH:MM:SS).
Base State: State of a logged in agent. These are the default states that are automatically set by the system.
Digital State: Digital state of a logged in agent.
Pending Disposition: Gathers data for those with pending dispositions.
State: Custom agent states as configured by customers.

**Common**
Account: Account or client name to display.
Account ID: Account ID is displayed.
Main Account ID: Main account ID is displayed.
Product: Displays product name.
Product Group: Shows products by group name.
Product Group ID: Product group ID number is displayed instead of the product name.
Product Group Type: Product group type of the Product.
Product ID: Displays products by ID number.
Product Type: Displays products by type.

**Custom Field**
Custom Field Name: Values generated by custom fields in IVR nodes. Learn more here.
Custom Field Name (String): Values generated by custom fields in IVR nodes, but converted to a number that allows us to aggregate the values.

**Interaction End Time**
Interaction End Half Hour: Timestamp when an interaction has ended, grouped by half-hour (30 minutes) increments.
Interaction End Hour: Timestamp when an interaction has ended, grouped by hour (60 minutes) increments.
Interaction End Quarter Hour: Timestamp when an interaction has ended, grouped by quarter hour (15 minutes) increments.
Interaction Start Time
Interaction Start Half Hour: Timestamp when an interaction has started, grouped by half hour (30 minutes) increments.
Interaction Start Hour: Timestamp when an interaction has started, grouped by hour (60 minutes) increments.
Interaction Start Quarter Hour: Timestamp when an interaction has started, grouped by quarter hour (15 minutes) increments.

**Lead**
Lead Aux 1: Shows additional lead information stored in Lead Aux one.
Lead Aux 2: Shows additional lead information stored in Lead Aux two.
Lead Aux 3: Shows additional lead information stored in Lead Aux three.
Lead Aux 4: Shows additional lead information stored in Lead Aux four.
Lead Aux 5: Shows additional lead information stored in Lead Aux five.
Lead City: Presents data for the lead’s city.
Lead Complete: Displays for leads whose status is complete.
Lead Country ID: Displays for the lead’s country ID.
Lead List: Displays for specific lead list names.
Lead List ID: Displays for specific lead list ID numbers.
Lead Max Passes: Displays for leads that have reached max passes.
Lead Pass Count: Shows the pass count of leads.
Lead State: Presents data for the lead’s states.
Lead Status: Displays for the status of leads, whether the lead is ready or complete.
Lead Success: Shows successful outbound calls tagged as ‘Success’ during dispositions.
Lead Timezone: Presents data for lead’s timezone.
Lead ZIP: Presents data for lead’s zip code.

**Segment**
Abandon Type: Displays long or short type of call abandon.
Actual Interaction End Time: Timestamp when an interaction has ended.
Actual Interaction Start Time: Timestamp when an interaction has started.
Actual Started Time: Timestamp when a call is started. Also called Call Started Time in the Interaction Details Report.
After Hours: Data of calls that came in after hours.
Agent Connected: Data of agents for when they were connected and handled a transaction or not.
Agent Disposition: Type of agent disposition data to display — default, requeue, or to not display at all.
Agent Disposition Notes: The notes in an agent’s disposition.
Agent Presented: Displays whether an agent was presented with calls or not.
Agent Rank: Shows the agent rank assigned.
ANI: Displays by ANI.
Avg Wait Time within Interaction Bucket: Average wait time bucket (0-9 seconds, 11-19 seconds, etc.) for interactions.
Avg Wait Time within Segment Bucket: Average wait time buckets (0-9 seconds, 11-19 seconds, etc.) for segments.
Call Result: Different call results such as inbound abandon or inbound defected, among many others.
Call Type: Inbound or outbound calls.
Channel Type: Voice or digital.
Complete: Complete or incomplete calls.
Contact: Agent dispositions marked as ‘Contact.’
Dial Type: Type of outbound calling.
DNIS: Displays by DNIS.
Duration Type: Length of call.
Final: Final segment of the call.
First Contact: Lists if segment is first contact.
Index: Number of the segments of a call.
Interaction Handle Time Buckets: Time intervals or buckets showing agent interaction handle times. Time intervals are by 60 minutes. (00:00 to 00:59, 01:00 to 01:59, etc.)
Outbound Caller ID Description: Shows the description added to outbound caller IDs.
Presented: Calls that were presented to an agent.
Recording URL: Provides the URL for phone call recordings.
Resolution Success: Customer issue was resolved successfully and customer did not return with the same issue.
Resolved: Calls marked as ‘Resolved.’
Segment End Time: The actual end time of a segment (HH:MM:SS).
Segment Start Time: The actual start time of a segment (HH:MM:SS).
SLA Passed: Shows calls that were answered by the agent within the threshold configured for the queue.
SLA Qualified: Presents data that passed SLAs. The SLA calculation won’t count short calls.
Success: Calls marked as ‘Success’ in agent dispositions.
Term Party: Identifies which party terminated the interaction.
Term Reason: Reason an interaction was terminated.
Termination Reason: Reason a call was terminated.
UID: Attribute for the last 16 digits of the UII (013VRU00000XXXXX).
UII: Displays a unique identifier for an interaction.
UII format: "YYYYMMDDHHMMSS013VRU00000XXXXX", where “YYYYMMDDHHMMSS” is the date/time stamp (DTS), “013” is a static value, “VRU” is the voice response unit (VRU) number, and “00000XXXXX” are random digits.
UII Date: Attribute for the date part of the UII (YYYYMMDD).
UII Time: Attribute for the time part of the UII (HHMMSS).
Unique Inbound Contact Bucket: Buckets of unique contacts made inbound interactions handled by an agent. For example, an agent that has 22 unique contacts will fall under the 21-25 bucket.
Note: The metrics for SLAs reported will be according to the settings that were in effect during the call. This means if SLAs are adjusted, this will be reflected in the report generated.

**Time**
Started Half Hour: Presents data for start time with options for every half hour.
Started Hour: Displays data for start time with options for every half hour.
Started Quarter Hour: Presents data for start time with options for every quarter hour or fifteen minutes.