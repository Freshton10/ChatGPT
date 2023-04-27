---
title: Scheduling reports in Historical reports
layout: layout-page-sidenav
description: Historical reports allow you to customize how you want data and reports sent to your preferred destinations. While Historical dashboards are always exported as PDF files, Historical reports can be exported as raw data (CSV files) or as spreadsheets (XLS files).
sub_collection_render: true
single_level_nav: true
_data: single-level-nav
collection_group: [Ringcentral]
sgts_collection_group: [toolchain]
sgts_layer_group: [base]
sgts_title: Scheduling reports in Historical reports
redirect_from:
    - https://support.ringcentral.com/article-v2/Scheduling-reports-in-Historical-reports.html?brand=RingCentral&product=EV&language=en_US
---


### Scheduling reports in Historical reports

You can arrange for your reports to be formatted for and delivered by:
Email: Sends reports through email.
File transfer (FTP): Uses File Transfer Protocol to send reports to your computer or server.
S3 bucket: Sends reports to your AWS cloud storage resource.
Secure file transfer (SFTP): Uses SSH (Secure Shell) File Transfer Protocol to send reports to your computer or server.
This article is about scheduling reports. Read this article to learn how to schedule or export dashboards.

**Accessing scheduled Historical reports**
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Click on your scheduled Historical report.
Learn how to create Historical reports.

**Creating a new schedule**
You can create a schedule in any of three locations.
In the Schedules folder
In a report folder (Standard, Shared, Private, and Favorites)
In the report’s viewer mode
Note: The data in your scheduled reports will be identical to the data that you see when you look at those reports in viewer mode. Learn more about historical analytics platform limits.

**Creating a new schedule in the Schedules folder**
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Click on the New schedule button in the upper right-hand corner.
In the General section, select the report you want to schedule in the Report name dropdown.
Add a custom name for your scheduled report in the Schedule name field.
Select your preferred file type in the File type dropdown.
Add a custom name for your report in the File name field.
In the Schedule section, select how often you want the schedule to run in the Frequency dropdown, then fill out the rest of the field options.
In the Destination section, select your preferred destination in the Destination type dropdown, then fill out the rest of the field options.
Click Save and close or Save.
Note: In the Schedule and Destination sections, settings may change according to the selected frequency and destination type.

**Creating a new schedule in the report folders**
Sign in, then click on the Analytics icon.
Go to Historical reports and select the folder where the report you want to schedule is located. (Standard, Shared, Private, Favorites)
Click the Actions icon to the far right of the report you want to schedule, then select Schedule from the dropdown.
In the General section, select the report you want to schedule in the Report name dropdown.
Add a custom name for your scheduled report in the Schedule name field.
Select your preferred file type in the File type dropdown.
In the Schedule section, select how often you want the schedule to run in the Frequency dropdown, then fill out the rest of the field options.
In the Destination section, select your preferred destination in the Destination type dropdown, then fill out the rest of the field options.
Click Save and close or Save.

**Creating a new schedule in the report’s viewer mode**
Sign in, then click on the Analytics icon.
Go to Historical reports and select the folder where the report you want to schedule is located. (Standard, Shared, Private, Favorites)
Open the report you want to schedule. Click the Actions icon in the upper right-hand corner, then select Schedule from the dropdown.
In the General section, select the report you want to schedule in the Report name dropdown.
Add a custom name for your scheduled report in the Schedule name field.
Select your preferred file type in the File type dropdown.
In the Schedule section, select how often you want the schedule to run in the Frequency dropdown, then fill out the rest of the field options.
In the Destination section, select your preferred destination in the Destination type dropdown, then fill out the rest of the field options.
Click Save and close or Save.
A new schedule created in viewer mode will only display saved or applied filters created in edit mode. Learn more about using filters to edit your reports.

**Schedule settings**
General
Report name: Dropdown that contains all existing reports available to you. Learn more about creating Historical reports.
Schedule name: Name of the schedule you are creating.
File type: CSV (default) or XLS.
File name: Customize the name of the CSV or XLS file you will receive. By default file name includes the report name, run time, and timezone (File name_mm.dd.yyyy_hh-mm_TZ).
Note: If you don’t customize the file name, the name of the selected report will be used (“Report name_mm.dd.yyyy_hh-mm_TZ”)

**Schedule**
Settings under the Schedule section change according to the frequency type chosen.
Frequency type: Select how often you want the report sent to your destination.
All working days
Custom
Every day
Every hour
Every Monday
The first of the month
Run time: Set the time (hh:mm AM/PM) at which you want your report to be sent (default: 9AM).
Starts: Set the date (mm/dd/yyyy) on which you want your report to start being sent (default: current day).
Ends: Set the date (mm/dd/yyyy) on which you want your report to stop being sent. Keep this field empty to keep sending the report until you deactivate it.
Timezone: Select the timezone in which you want the schedule to run.
Pacific Time (US & Canada)
Mountain Time (US & Canada)
Central Time (US & Canada)
Eastern Time (US & Canada)
Hawaii
Repeat: Set the frequency with which you want to run your report (default: Daily).
Run every: Select, in conjunction with the Repeat setting, the number of times you want your report to run. (Available only in Custom frequency.)
For example, if you want your custom report to run twice a month, select Monthly in the Repeat setting and select ‘2’ in the Run every setting.

**Destination**
Settings under the Destination section change according to the destination type chosen. Email is preselected as the default destination.
Email: Sends reports as email attachments.
Subject: Write the subject line of the email to which your Historical report will be attached (default subject: Schedule). You can change the subject as you wish.
Destination email(s): Choose one or more destination email addresses. Separate multiple addresses by using a comma or hitting the Enter/Return key to create a new line.
Message: Customize the short email message to accompany the report (The default text message : “Hello, Your scheduled email is ready”). Your message will be added before the default text. (Default: “You can download the report in attachments. To view the interactive version of the report, please visit Engage Analytics.”).
Sender email: Write the email address of the email sender server for the scheduled report. (Default: engage.analytics@ringcentral.com).
Note: Customizing the sender email will only affect the scheduled report you are configuring.
File transfer (FTP): Uses File Transfer Protocol to send reports to your computer or server.
FTP server: Enter the URL of your FTP server.
FTP username: Enter the username of your FTP server’s user.
FTP password: Enter the password of your FTP server’s user.
FTP directory: Enter the directory’s full path on your FTP server where you want to store your report.
S3 bucket: Sends reports to your AWS cloud storage resource.
S3 URL: Enter the URL of your S3 bucket. Formatting options include:
http://s3.[region].amazonaws.com/[bucket-name]/
http://[bucket-name].s3.[region].amazonaws.com/
https://s3.[region].amazonaws.com/[bucket-name]/[key-name]
https://[bucket-name].s3.[region].amazonaws.com/[key-name]
https://[bucket-name].s3-[region].amazonaws.com/[key-name]
Note: Please specify your preferred region in the AWS settings to use S3 URL with the region.
S3 Access Key ID: Enter the Access Key ID of your S3 bucket.
S3 Secret Access Key: Enter the Secret Access Key of your S3 bucket.
Secure file transfer (SFTP): Uses SSH (Secure Shell) File Transfer Protocol to send reports to your computer or server.
SFTP Server: Enter the URL of your SFTP server.
SFTP username: Enter the username of your SFTP server’s user.
SFTP password: Enter the password of your SFTP server’s user.
SFTP directory: Enter the specific location of the directory’s full path on your SFTP server where you want to store your report.

**Editing an existing schedule**
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Locate the schedule.
Search for your scheduled Historical report in the search bar
OR
Click the Show my schedules toggle to the right of the search bar.
Click on your scheduled Historical report.
On the settings page, edit the settings you want to change.
Click Save and close or Save.
Note: You cannot edit scheduled Historical reports that other users have created. Contact the owner of the schedule to make any changes. 

**Cloning an existing schedule**
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Locate the schedule.
Look for the scheduled Historical report that you want to clone manually
OR
Search for the scheduled Historical report in the search bar.
Click the Actions button at the far right of the report’s row.
Select Clone.
Select the historical report you want to clone and choose a name for the cloned report in the Clone schedule window. (Default: ‘Clone of: report name.’)
Click Save.
On the configuration page of the cloned report, change some settings, if you wish to do so.
Click Save.
If you click Go to report, a new tab will open that will take you to the report’s page. If a report is set to private, the Go to report option will not appear in the menu.

**Deleting a schedule you’ve created**
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Locate the schedule.
Search for your scheduled Historical report in the search bar
OR
Click the Show my schedules toggle to the right of the search bar.
Click the Actions button at the far right of the report’s row.
Select Delete.
Note: You cannot delete scheduled Historical reports that other users have created. Contact the owner of the schedule to make any changes. If the owner of the schedule cannot be reached, contact your account manager.

**Testing a schedule**
Testing a schedule helps in making sure the right fields and credentials are correct.
Sign in, then click on the Analytics icon.
Go to Historical reports > Schedules.
Locate the schedule.
Search for your scheduled Historical report in the search bar
OR
Click the Show my schedules toggle to the right of the search bar.
Click the Test run button at the far right of the Destination section.

Testing a schedule will yield either a success message in a green notification, or an error message in a red notification.
Depending on the destination, check the following:
Email
Check if the email address is correct.
Check if there are no issues with the email server.
S3/FTP/SFTP
Check if the server credentials are correct.
Check if there are no issues with your server.
Check if the user has rights to upload files to your server.
Note: All mandatory fields must be filled, and all errors must be fixed before continuing the test run or saving the schedule.
