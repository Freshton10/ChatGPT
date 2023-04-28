---
title: Studio training
layout: layout-page-sidenav
description: Studio is a user-friendly application that allows you to create, edit, and maintain scripts for routing in your Contact Center. Studio scripts can be used for self-service (IVR) as well as for the media types, or channels, in your RingCentral Contact Center system. These channels can include self-service (IVR-only); inbound phone, chat, or email; automated outbound phone, chat, or email; and work items. Contact routing scripts for these channels can also incorporate IVR actions and multiple branches based on those actions. The following image shows a simple script that allows callers to route to an agent or to leave a voicemail, and that plays music while the caller is on hold or waiting for an agent.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Studio training
redirect_from:
    - https://support.ringcentral.com/article-v2/Studio-training.html?brand=RingCentral&product=CC&language=en_US
---

### Studio training

Studio is a user-friendly application that allows you to create, edit, and maintain scripts for routing in your Contact Center. Studio scripts can be used for self-service (IVR) as well as for the media types, or channels, in your RingCentral Contact Center system. These channels can include self-service (IVR-only); inbound phone, chat, or email; automated outbound phone, chat, or email; and work items. Contact routing scripts for these channels can also incorporate IVR actions and multiple branches based on those actions. The following image shows a simple script that allows callers to route to an agent or to leave a voicemail, and that plays music while the caller is on hold or waiting for an agent.

Studio scripts can be very basic or extremely complex, depending on the needs of your organization. The application includes more than 150 pre-defined routing components known as actions, and these actions can be combined in thousands of different ways. Many actions have the ability to incorporate variables, and this further extends the application's capabilities and flexibility. Custom integrations may also be available. Drag-and-drop functionality and a visually-intuitive interface ensure that Studio remains easy to use for both novice and experienced workflow designers.
To use Studio, you must download the application from Central. Once the application is installed, you can log in to Studio using your Central credentials. You cannot have a different username or password for Studio, and you should always manage your credentials (for example, change your password) in Central.
If your organization has more than one business unit, you must use the credentials for the business unit you were logged into when you downloaded Studio. This situation may apply, for example, to Business Process Outsourcers (BPOs) who have separate business units for each of their customers.
**Requirements**
Windows .NET Framework version v4.8 or later.
Windows operating systems.
The scripter's CXone security profile must include Studio permissions.
**Features**
You can perform some basic tasks related to scripts from within CXone, but to create, manage, and test scripts, you must use Studio.
If you have any issues with Studio being falsely identified as 'infected,' contact your antivirus vendor.
Documentation for supported APIs is available upon request.
To share ideas and collaborate with other scripters, you can visit the RingCentral Community site. Contact your account representative if you do not have access to the community.
**Definitions**
Studio has a graphical interface that lets you create basic scripts with minimal knowledge of scripting languages. This section provides a high-level introduction to the basics of scripting in Studio. You can also follow this tutorial to create a basic script in Studio.
**Script types**
There are different script types in Studio. Each type corresponds to a kind of routing in CXone. When you create a new script, you must select the correct script type. Some actions only work with certain script types. For example, ASR-related actions only work with Phone scripts. The Studio script types are:
**Actions**
The basic building blocks of Studio scripts are the actions. Actions are how you add specific functionality to your script. There are hundreds of actions in Studio. The Actions section of the online help contains topics for most of the actions. You can access online help for an action directly from Studio by selecting the action and pressing F1 on your keyboard.
Studio provides hundreds of different actions, and each action performs a process of some kind. Examples include: collecting data, playing a message or music, checking to see if a phone number is in the do not call (DNC) list, providing menu options to the caller, and so on. Studio actions reside in both the Framework tab and the Tools tab.
**Branches**
Branches are used when an action has two or more possible outcomes. They divide the script into the paths that the contact might follow, and help you create the workflow your organization requires. When connecting one action to another, the PickBranch box opens for you to select (or create) the type of branch that a contact will take under certain circumstances. For example, selecting the Error branch will direct a contact along that branch when an action fails to execute properly.
**Connectors**
Connectors are how you link actions and create the flow of your script. On the canvas, connectors appear as thin lines with arrows on them that connect two actions. You can bend and curve connectors to move them around other actions on the canvas.
**Audio prompts**
Audio prompts are a fundamental aspect of many scripts. These are audio files that the script plays to provide information to the contact or ask the contact to make a choice or input information using their phone. You can learn how to manage prompts in Studio, including using text-to-speech or recording your own audio prompts to use in scripts.
**Snippet scripting language**
Snippet is the in-house scripting language used for all custom scripting needs in Studio. Custom scripting isn't required, but it helps you fine-tune your scripts to achieve the workflow your organization needs. You can learn about Snippet if you need to use it to customize your scripts.
**Properties**
Display an action's properties by right-clicking on an action to open the Properties box, or left-clicking to highlight and open the Properties tab. The action's properties include branch options and offer customization parameters such as identifying a specific skill or entering text to appear as a message to an agent.
**Additional configurations**
Some actions have additional configuration options that you can access/launch by double-clicking the action. For example, double-clicking the Play action opens the Play Properties box, allowing you to record an audio prompt.
**Installing Studio**
You may want to double-check your browser or antivirus software settings to ensure that Studio is allowed to be downloaded and run. Contact and work with your antivirus vendor if you experience any issues. For example, Panda Cloud Antivirus is known to block Studio downloads; if you have the Panda antivirus program, visit the Panda Security website and search for "modifying internet connection permissions" for more information on configuring Panda to prevent this. Perform the following steps to download and install Studio:
Click on your Profile Icon at the upper right.
Go to Support & Downloads > Software and Updates.

A webpage will open: https://downloads.incontact.com/
Scroll down and find Studio, click Download.

Run the application and proceed with the software Installation.
When the login window appears, enter your credentials to access Studio. The User field is pre-filled with your platform username.
Note: Studio prompts you to automatically update as RingCentral Contact Center releases new features, hotfixes, and so forth. An archived Studio version will remain in your local folder after each update for potential diagnostic reasons.
**Signing in**
Open the Studio.Enter your login credentials.
For Central Accounts, just use Standard login and enter your Contact Center Credentials.

For Userhub Accounts, you need to use Login with Session ID. To get your Session ID, you must be logged in to Contact Center Portal. Click on the Applications and click Studio Authentication. Click OK on the popup window and the system will copy the session ID to your clipboard.


Note: Your security profile must have Studio access Enabled. And login via SSO is not yet supported.
