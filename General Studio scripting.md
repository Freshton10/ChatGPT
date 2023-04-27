---
title: General Studio scripting
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: General Studio scripting
redirect_from:
    - https://support.ringcentral.com/article-v2/General-Studio-scripting.html?brand=RingCentral&product=CC&language=en_US
---


### General Studio scripting

Scripting in Studio allows administrators to create the IVR flow: menu, hold music, calling routing method, etc. Our RingCentral Contact Center implementation team works with the administrator to build out the entire flow. 
When customers encounter issues with their scripting, support will refer them to the implementation team. 
Note: The customer will have to pay a fee to RingCentral or Nice/InContact’s implementation team depending on the issue. 
To reach our implementation team for scripting, please contact your RingCentral Contact Center sales representative. If you’re a new customer, you can fill out the form on our overview page.

**Best practices**
When determining how to script your IVR flow, some best practices to keep in mind are to:
Mitigate risk
Promote scalability, flexibility, and reusability
Focus on uniformity and maintainability
Comprehensive design that’s supportable, stable, and secure
Enable good agents and excellent customer experiences

**Additional scripting tips**
Port checker at the beginning of every entry script.
newSkill is used as a variable name for skill number.
skillName assigned in DNIS switch.
vmSkill is used as a voicemail skill variable.
Lang used as language variable. eng, spa, fre, etc.
{env} used as environment variable for DEV and PROD
promptPath variable for prompts
CheckAgents during queue music loop.
ReqAgent is for removing the call from the queue before any transfer, VM, or RunScript out of the Queue.
Always return from RunSubs. Never RunScript, Queue a call, or transfer out of a RunSub.
Do not RunScript out of a Queue unless you remove the call from the queue.
Connect music actions to a .5 second wait before looping them back to music.
Always connect default branches. Use DEFAULT in every Switch statement.
Always caption every action with a descriptive caption
Do not use a hang-up after the OnRelease event.
Spawn all logic that comes after OnRelease.
All Spawned scripts require an End action after the script logic is complete.
Use unique Loop counters.
Keep your scripts tidy with uniform spacing. Scripts should flow horizontally. Avoid diagonal and crossing lines.
Always build a custom personal queue. If there is a screen pop, you should be copying the screen pop logic to the CPQ and passing appropriate params.
OnReskill should follow queue logic (check agents, music, etc.)

**Agent scripting**
Agent scripting is written text presented to an agent through their interface (ex., MAX or Salesforce) or a screen pop, assisting the agent in responding to a caller or other contact.
Admins can create and define agent scripting using through Studio. The script will then display in a pane of the agent window.

**DNC Add via Group**
Adds a phone number to the DNC group, which a skill or a business unit can then reference.
Note: This is only applicable for Phone type scripts.
