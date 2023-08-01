# Login Data Report

## Description
This is a non-context sensitive report that builds a single sheet excel file of user login data over the past 90 days. The report gathers information such as the login attempt status, the login attempts username, the license type of said user, the login and logoff time in UTC time and the logged in session duration. The time duration of how far the report will check can be modified by adjusting the hours values on line 421.

Please note that this data itself is suspect due to the fact that logoff time is not accurate. The logoff timestamp can be either a user directly selecting the logoff button, the session timing out, or a user closing their browser.

## Preview Image
![Report Preview](Preview.png)

## Installation Instructions
1. Go to the Admin section of Jama
1. Click the Reports tab
1. Click Add Report
1. Fill in the Add/Edit Report form as shown below.
1. Click Save

![Report Configuration](config.png)

## NOTES: 
- Your Organization field will have a different value.  
- Rename the report to anyting you like
- Enable any report format that you'd like to use

## Running the Report
1. Go to the Project section of Jama
1. Click Reports
1. Select the report name you specified when installing the report.
1. Click Run Report
