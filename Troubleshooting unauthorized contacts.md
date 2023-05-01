---
title: Troubleshooting unauthorized contacts
layout: layout-page-sidenav
description: The “Unauthorized contacts'' error appears when an agent places a call to a number and receives a suppression calling script in return. This error typically occurs when the number that the agent has dialed has been placed on the Do Not Call (DNC) registry, or on an internal Contact Center list that specfies that the number not be called.
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Troubleshooting unauthorized contacts
redirect_from:
    - https://support.ringcentral.com/article-v2/Troubleshooting-unauthorized-contacts.html?brand=RingCentral&product=CC&language=en_US
---

### Troubleshooting unauthorized contacts

**Check for suppression script**
Go to the Contact Center and log in.
In the left-hand navigation bar, click ACD.

Click the dropdown arrow next to Outbound Skills, then click Skills Control.
Select the Call Suppression tab and see if there is a suppression script in the flowchart. If there isn’t one, check the DNC list.
To check the call suppression list, you must open the script in the Studio application and open the Snippet action to see the list.
Log in to the Studio application (Windows only).
Choose the call suppression script from the Browse list on the far right. 
Double click to open the script and locate the Snippet action to see the list of numbers being blocked.

Note: The structure and logic of the suppression script may differ for each account.
**Check the DNC List**
Follow these steps to confirm that the unauthorized contact number is on the DNC list.
Go to the Contact Center and log in.
In the left-hand navigation bar, click ACD.
Click the dropdown arrow next to Lists, then select DNC.
Click on the DNC list to bring up its details page. 
Click Download, then open the downloaded Excel sheet to search for the number. 
If the number is not in the DNC or call-suppression list, you will need to create a case with RingCentral Support.
**How to Update the Do Not Call List**
Log in to Contact Center.
On the left-hand side, expand the Lists menu.
Click DNC.
Click on the file you want to update.
Under the Details tab, click on Download (on the righthand side) and select Active Only.
Once the .csv file has been downloaded, update it then save as a new file.
Make sure the file name is not the same (e.g., original file name DNC then new file name DNC 1) and keep it simple.
Back in the file you had opened in Contact Center, click on Select File (in the top right-hand side).
Select Upload New then click on Browse to select the updated list.
Click Next.
Set the Field Mapping and click Next.
Once List Processing is finished, click Done.
Notes:
You can also add numbers to the DNC list by dispositioning a call with a DNC disposition.
DNC records can not be removed from the DNC list, but it can be updated by adding an expiration date/time to the records available for calling.
