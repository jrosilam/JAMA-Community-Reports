<h1>User Login Activity and Event Report</h1>
<h2>Description</h2>
<p>This report gathers User Login Activity and User Events for a selected time frame, and outputs an Excel multisheet report.

On the first sheet, “Login Activity”, the report builds a row per user, showing login stats, like how many login activities, and the latest login activity.
  *Please note that this data itself is suspect due to the fact that logoff time is not accurate. The logoff timestamp can be either a user directly selecting the logoff button, the session timing out, or a user closing their browser.*

On the second sheet, “Event Activity”, the report builds a parent row per user, followed by child rows per “Event”, across all projects of the organization, triggered by that user.
Events are primarily Create, Update, and Delete activities. (Login events are excluded intentionally on the “Event Activity” sheet, because they are accounted for on the first sheet).

Because “Event Activity” data can be extensive, it is beneficial to filter the report by User Name (Full Name) when selecting large time parameters. 
If the Report Runner would like to narrow in on particular “Event Activity” to reduce data returned, reach out to the report team or if you are a CSM or Consultant the [ eventEnumList ] and [ objectTypeEnumList ] can be modified on line 239.
</p>

<h3>Preview Image Sheet 1: "Login Activity"</h3>

![Login_Activity](https://user-images.githubusercontent.com/99203913/210880285-92768c46-3f53-4273-bcc3-c34da68de390.png)


<h3>Preview Image Sheet 2: "Event Activity"</h3>

![Event_Activity](https://user-images.githubusercontent.com/99203913/210880319-07126b08-0368-44d8-ab17-bdaf8b6eb950.png)

<h1>Installation Instructions</h1>
<ol>
  <li>Go to the Admin section of Jama</li>
  <li>Click the reports tab</li>
  <li>Click add report</li>
  <li>Fill in the Add/Edit Report form as shown below</li>
  <li>Click Save</li>
</ol>
<p>Helpful description to add at install: <em>Check one time parameter and the report will show data from the date the report is run. Outputs a two sheet Excel report with tabs: "Login Activity", "Event Activity". Filter by User Name, considering larger time parameters.</em></p>

![InstallReport png](InstallReport.png)

<h3>Report parameters:</h3>

|Data Type|Display|Name|
|----------|---------|--------|
|Boolean|One Week| reportA_oneWeek|
|Boolean| Two Weeks| reportB_twoWeeks|
|Boolean| One Month| reportC_oneMonth|
|Boolean| Three Months| reportD_threeMonths|
|Boolean| Six Months| reportE_sixMonths|
|Boolean| One Year| reportF_oneYear|
|String Parameter| User Filter (Full Name)|reportG_userFilter|

 <h2>Report Run Instructions</h2>
 <ol>
  <li>Log into the Organizations Instance</li>
  <li>On the top right nav of project dashboard select "Reports" dropdown</li>
  <li>Select the "User Activity and Event Report"</li>
  <li>Select a time parameter</li>
  <li>If filtering the report by user enter String value- first and last name (not case sensitive)</li>
 </ol>
 
 ![RunReport png](RunReport.png)

 
  
