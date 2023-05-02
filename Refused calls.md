---
title: Refused calls
layout: layout-page-sidenav
description: A refused call is one that the RingCentral Contact Center system sends to an agent but that the agent doesn’t answer.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Refused calls
redirect_from:
    - https://support.ringcentral.com/article-v2/Refused-Calls.html?brand=RingCentral&product=CC&language=en_US
---

### Refused calls

**What happens when a call is refused?**
The call is pulled back from that agent and presented to the next available agent.
Note: The caller won’t know that their call is refused. If hold music is playing, it will continue playing until an agent picks up the call, even if there are multiple refusals.
The agent who refused the call is put in an unavailable Refused state. The agent will need to manually change their state to Available.
The refused call will appear on various reports, some of which indicate the agent that refused the call. Learn more about refusal reasons in the Contact History Report.
**What can cause a refused call?**
Most obviously a refused call occurs when an agent doesn’nt answer a call, but there are other causes, as well. For example, the agent may have logged into MAX Agent with an invalid phone number.
Below are some examples of refused calls and how to resolve them, if possible.
**Call refusal on MAX**
Inbound and outbound calls won’tt connect, and will show as refused (calls come in, do not connect, then show refused). Agents notice calls being delivered but then refused.
**Possible causes:**
The Station ID field for Caller ID is invalid.
The agent’s RingCentral extension call-forwarding settings are set to only one ring.
There’s not enough time for the device to ring before forwarding the call to an offline deskphone.
The call may be forwarded to an offline or unused device.
**Resolutions:**
Confirm the Station ID login number. If the number entered in the Station ID field under Caller ID is invalid, the system will reject the attempt.
Make sure that the extensions call-handling and -forwarding settings leave enough time for the device to ring before forwarding. Adjust call forwarding rings to allow for at least four rings / 20 seconds.
**Note:**
Always use a valid number that you own as your Caller ID.
Caller ID can be set at the Business Unit or Station levels. (A Station setting will override any Business Unit settings.)
**Cause codes**
When refused calls are pulled into the Central Contact History Report, users may see cause codes, which indicate the reasons for refused calls. 
Note: The Refusal Reasons column will appear in the report only if you check the Display Extended Data box in Report Options, then run the report.
**High volume of call refusals using mobile phones**
Agents may experience a high volume of refused calls when using mobile phones for the agent’s leg. In some cases, they may not even hear the phone ring before the call is refused. 
**Possible causes:**
Mobile carrier returns a “ringing” or “session progress” response before actually alerting the mobile subscriber of the incoming call.
The mobile carrier sends the response, then attempts to locate the subscriber on their network, and once located, the subscriber of the incoming call alerts the subscriber. The time to locate the subscriber on the mobile network varies, but it has been observed in some cases to take up to 18 seconds. The mobile carrier does this to prevent the caller from hearing dead air while waiting for the subscriber to be located and alerted of the call. This causes the RingCentral Contact Center platform to start the no-answer refusal timer before the end-user knows they are receiving a call. Not all carriers do this, but some do.
Mobile carriers take too long to find the subscriber without returning a “ringing” or “session progress” response.
This causes RingCentral Contact Center to cancel the call early because the platform is looking for a response after the "trying" response but does not receive one within an appropriate amount of time.
The agent has their mobile phone on silent mode.
The agent’s phone is in power-saving mode.
**Resolutions:**
Plug the mobile phone into power and take it out of standby, so the screen never turns off.
If available, activate and use WiFi calling. This ensures that the provider’s gateway always has an accurate route for the mobile device cached. WiFi calling results in decreased time to locate and alert the mobile device.
Increase the timeout for no answer refusals to 36 seconds. This gives the carrier more time to locate and alert the mobile subscriber on their network before the RingCentral Contact Center no answer refusal timer is reached.
Note: The mobile user may need to contact their provider to confirm that their pre-voicemail ring duration can be extended.
Make sure that the phone isn’t in silent mode, and that the ringer volume is audible and comfortable.
Disable power saving mode or connect the mobile device to power.
**Possible causes with no known resolutions:**
Low-quality / no mobile signal
Carrier routing issues
