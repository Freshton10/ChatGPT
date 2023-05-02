---
title: Installing and integrating Agent in Central for Oracle Service Cloud
layout: layout-page-sidenav
description: 
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Installing and integrating Agent in Central for Oracle Service Cloud
redirect_from:
    - https://support.ringcentral.com/article-v2/Installing-and-integrating-Agent-in-Central-for-Oracle-Service-Cloud.html?brand=RingCentral&product=CC&language=en_US
---

### Installing and integrating Agent in Central for Oracle Service Cloud

The Central environment will reach End of Life on December 31, 2024, and will no longer be supported. You must convert your account to the User Hub environment that replaces Central. Learn how
Note: This article does not apply to Engage customers.
Install and configure the RingCentral Contact Center Agent for Oracle Service Cloud to employ the functionality of the Contact Center agent in conjunction with your company's Oracle database. The typical installation and configuration process takes approximately 15–30 minutes. See your Oracle documentation for help using or troubleshooting the Oracle Service Cloud product.
You must use Internet Explorer or Legacy Microsoft Edge (not Chromium Edge). The application does not run on Chromium Edge, Chrome, or Firefox; Agent for Oracle runs in the Oracle Service Cloud Product.
You may raise a ticket with Oracle to increase the upload size for add-ins to accommodate the 65MB audiocodes add-in.
Click the app selector and select ACD.
Go to Support > Software & Updates.
Read the agreement and click Accept.
Locate and click inContact_Agent_Oracle_Service_Cloud.zip to begin the download.
Open the folder once the download is complete.
Locate and click NICEinContact-CXoneAgent-OracleServiceCloud-InstallConfigure.docx.
Follow the instructions to configure your account.
To fully integrate the Contact Center agent with Oracle Service Cloud, you need to install CTI add-in files, import CTI custom objects, and import a custom report. You also need to grant access to these things to users.
Agent for Oracle Service Cloud has two available agent views: classic view and consolidated view.
**Installing CTI add-ins for classic view**
The Contact Center agent for Oracle Service Cloud classic view provides an agent interface integration between the RingCentral platform and the Oracle Service Cloud CRM.
Under Navigation, click Configuration > Site Configuration.
Double-click Add-in Manager.
Click New > Compressed Add-In Files in the file search dropdown.
Double-click the NICEinContact.Cti.zip file from the add-ins directory.
Using the same process, add the NICEinContact.Cti.Admin.zip file.
Click Save in the top toolbar to import the add-in files.
**Installing CTI add-ins for consolidated view**
The Contact Center agent for Oracle Service Cloud consolidated view removes the media bars for a streamlined agent experience.
Under Navigation, click Configuration > Site Configuration.
Double-click Add-in Manager.
Expand Agent Desktop Add-Ins.
Double-click the NICEinContact.CXoneAgent.zip file from the add-ins directory.
Using the same process, add the NICEinContact.CXoneAgent.Admin.zip file.
Click Save in the top toolbar to import the add-in files.
**Granting add-in access permissions**
Once the add-in files are installed, you can grant access permissions to users to access individual add-ins. All the agents who handle contacts need access to the inContact.Cti or the NICEinContact.CXoneAgent add-in. Only grant permissions to the inContact.Cti.Admin or the NICEinContact.CXoneAgent.Admin add-in to users who need administrative rights. Users who need administrative rights should also be granted permission to custom objects.
Grant access to agents and to users who need administrative rights.
To grant permissions to all agents to access the Contact Center agent interface:
Click NICEinContact.Cti.zip or NICEinContact.CXoneAgent.zip under the Add-In Manager.
Click Profile Access and select the boxes for the appropriate interface assignments.
To grant permissions to users who need administrative rights:
Click NICEinContact.Cti.Admin.zip or NICEinContact.CXoneAgent.Admin.zip under the Add-In Manager.
Click Profile Access and select the boxes for the appropriate interface assignments.
Click Save.
A user already logged in to Oracle Service Cloud must log out and log back in for access changes to take effect.
**Importing custom objects**
It is important to import custom objects to fully integrate the Contact Center agent interface with the Oracle Service Cloud.
Under Navigation, click Configuration > Database and double-click Object Designer.
Click Import.
Browse for and select the IC_Cti.zip file. Click Open.
Click Next.
Select the objects to import and click Next.
After the objects have been successfully imported, click OK.
Click Deploy.
Specify the date and time for deployment of the objects, or check Deploy Immediately. Type the email address for the confirmation email and click Deploy.
If you are satisfied with the deployment specifications, click Yes. Click No to return to specify deployment. The deployment runs at the specified time.
Upon completion, click OK to refresh the Object Designer.
**Granting access to custom objects**
Under Navigation, click Configuration > Staff Management and double-click Profiles.
Double-click anywhere on the line of a profile to open it.
Click Permissions.
Click Custom Objects. Locate the IC_Cti package and select the appropriate permission boxes.
Note: Agents only need Read permissions.
Click Save.
**Importing a custom report**
Click Analytics > Reports Explorer.
Click Public Reports > New Report.
Click Import Existing Report Definition when the New Report Wizard appears.
Browse to find the Contact Center Results.xml file, select the file, and click Open.
Save the file as "Contact Center Results."
