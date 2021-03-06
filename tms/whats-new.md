# What's New in the TMS

<span style="font-size:90%;"> <a href="/whats-new-toc.md">What's New in the other LODS platforms?</a></span>

----------------------------
## Released May 7 2020


### <span style="color:#0078d7;">Class Browser - Multiple Tag IDs in URL</span>

You can craft your Class Browser URL with multiple tags in it so the page loads with them automatically checked and the page filtered by them when it loads. 

For multiple tags without group reference, the URL structure is https://[site url]/class/browse?tagId,tagId&matchtype=1. The matchtype is optional. If you leave it off, Match All will be checked. If you include it, use 0 for Match All and 1 for Match Any.
 
For a tag in a specific group and a tag in any group, the URL structure is https://[site url]/class/browse?groupIdtag,tagId. Use the group Id for the specific group in which you want the tag to be checked.

### <span style="color:#0078d7;">Find Lab Instances - Company Filter/Output Option</span>

Need to see your students’ lab instances by the company they belong to? You can do this using the new the new Company output option on Find Lab Instances. This column will display the company set in the user’s profile. You can also narrow the results to see only lab instances from a specific company’s users with the new Company filters available, Choose Company or Company Name. 

> ![](https://github.com/LearnOnDemandSystems/docs/blob/master/tms/images/FindLabInstances-CompanyFOO.png)
 
### <span style="color:#0078d7;">Instructors in All Sessions of Class Automatically</span>

Now when you set up a class with multiple instructors, all instructors will be automatically added to all sessions of the class. In addition, if you add an instructor later, they are also automatically added to all sessions. If you add another session, all instructors are added to it. When you remove an instructor from one or more sessions, they will not be re-added unless the you click Add all instructors to all sessions in the Instructors section of the class. 

### <span style="color:#0078d7;">Position of HTML Description on Courses</span> 

Want the HTML Description on your courses to be easier to see? This section is now at the top of the Course Profile page, directly below the Description, if present. The HTML Description section will be expanded by default. 

> ![](https://github.com/LearnOnDemandSystems/docs/blob/master/tms/images/CourseHTMLDescription.png)

### <span style="color:#0078d7;">Disabled Class Activities Re-enabled at Class End</span> 

Do you or your instructor’s forget to re-enable class activities at the end of class? No worries. Now, if the course is set to allow activities to be auto enabled after class ends, any activities disabled for students in a class will automatically be enabled for them when the class ends.

> ![](https://github.com/LearnOnDemandSystems/docs/blob/master/tms/images/ClassActivitiesReenabling.png)

### <span style="color:#0078d7;">Accessibility Items</span> 

Two improvements have been made to assist users with accessibility needs.
1. Users can now use the keyboard to access the pagination elements of search pages to pull up different pages of results.
1. The contrast ratio for the Incorrect Username and Password message on the login page has been increased to help with visual clarity.

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>

1. Class Browser/Course Catalog/On-Demand Browser. We have improved the filter functionality on these pages to not allow a change in filters until the previous filter results are loaded.

1. Tab alignment on Create/Edit pages. Tabs on the second row of an entity's Create/Edit page now stay properly aligned and do not move over to be underneath the selected tab.

1. Featured Date Chooser in User's Date Format. The Date Chooser will now input the date, using the browser setting of the user, into the Featured field in the Create/Edit Course page.

1. Percent Complete Column for New Students. The Percent Complete column will now appear correctly for new students added to a class roster.

----------------------------
## Released April 23 2020

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>

1. API – Calls for GetCourse and GetCourseByExternalID have had the new Date/Time values added to display in seconds rather than milliseconds. 
1. Class – Class activities now have a disable all check box to disable or re-enable all activities at once. Once any activities are disabled by the instructor, they cannot be launched by students but now remain available for class instructor(s) to use. This allows instructors to demo labs or prepare future activities while preventing students from skipping ahead in the curriculum.
1. Class – A Custom Virtual Meeting Host issue has been corrected. When setting the delivery to use a Custom Virtual Meeting and inputting a URL for the meeting, if the delivery was reset to Physical, the Enter Classroom button still displayed. Changing a class delivery back to Physical no longer displays the Enter Classroom button to users.
1. Class – Zoom’s integrated Virtual Meeting Host will now reflect the correct time in UTC for when a class is scheduled. It was picking up the user’s time zone as the UTC time for the event. Zoom does straight UTC and does not take into consideration daylight savings time. Therefore, if a class is scheduled right now for 8:00 Central Daylight Time, it will appear in Zoom as 13:00 UTC instead of 14:00 UTC. 
1. Class import – The “Inherit certificates from course” setting was not being enabled by default for classes when they were created through the class import. This prevented completion certificates associated with the course to be set up automatically on the class. The setting is now enabled by default when classes are imported.
1. Enrollments – On the Find Enrollments page, when using the Class Status filter and filtering for Any, it was not showing any search results. It now shows results for all statuses. 
1. Course Assignments – The Find Course Assignments page has had several updates. The Payment Type filter now has options for Is, Is Not, and Is or Is Not. Columns for Payment Type and Completion Status are now sortable. 
o	Sorting on the Payment Type column groups by types of payments but not within types. For example, a listing in the column may be Payment Type “Subscription” with the “Subscription Name”; it will sort Subscriptions together but does not sort by the name of the subscription. 
1. Labs – On the Lab Details page we have relabeled the button that cancels a lab instance to read Cancel instead of Delete. The delete label was confusing to some users.
1. Badges – On the Class Roster page, when a badge is added for an individual by clicking the trophy icon on the roster, a Badge chooser dialog opens to select the badge(s) to add. When the badge is added a message will briefly display on the roster line for the student that the badge was successfully added. The success message which showed in the chooser dialog has been removed. 
1. Chrome browser back button – A search issue in Chrome has been corrected, you can now use the Back button to return to a search page and have it return results. The issue was that on any “Find” page, if you ran a search, navigated away, then used the Back button to return to the search and run it again, you would receive an error message.  

----------------------------
## Released April 10 2020

### <span style="color:#0078d7;">Use Zoom for your Integrated Virtual Meeting Host</span>

Zoom can now be integrated in the TMS, allowing you to schedule a class and create the Zoom meeting all at once. The integration also gives each student links to class recordings directly from their enrollment. 

For information about how a Zoom integration functions, click here and for information about setting up a Zoom integration, click here.

### <span style="color:#0078d7;">Enable or Disable Class Activities</span>

You can control when and if students have access to class activities. Instructors can enable or disable any activity in a class they teach. Operations managers can disable activities in classes they manage. This allows blocking students from launching labs requiring an Azure pass. 

The course controls if activities can be disabled in a class. Courses default to not permitting activities to be disabled. When a course allows for activities in a class to be disabled, then any class using that course shows an Enabled check box on activities. All activities in a class, labs, external links (video, document, website), assessments, and SCORM modules can be disabled or re-enabled during class. Surveys cannot be disabled.

In the class, all activities are enabled by default. Instructors and operations managers have a check box on each class activity to disable or re-enable it. Uncheck the Enabled box to disable the activity. Students will see the update to the status of the activity within 30 seconds without refreshing the page. 

> ![](https://github.com/LearnOnDemandSystems/docs/blob/master/tms/images/enable-activity.png)

A disabled activity displays, slightly grayed out with a “Disabled by Instructor” message for students and the Launch button does not display.

> ![](https://github.com/LearnOnDemandSystems/docs/blob/master/tms/images/student-disabled-activity.png)

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>

1. Edit Class – We have corrected the prohibition from editing a class after it has started when the date has not been changed. Users were receiving a message, “You don't have the necessary permissions to set this class’s start date prior the current date and time." when they attempted to update fields other than the class start date and save a class.

----------------------------
## Released April 02 2020 

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>

1. API – We added some return values to several API calls. The SearchLabInstances call now returns the LastActivity value. The GetCourse and the GetCourseByExternalId calls now include values for CourseDateCreated and CourseLastModifiedDate.
1. Date and Time formats – We have updated the date formatting to configure based on the browser’s language setting rather than only show in US date format of MM/DD/YYYY. 
1. Classes – We have modified classes so that the start date and start time must be equal to or later than the user’s current date and time. 
1. Training Key Pools - Ops Managers are no longer able to create a Training Key Pool using an archived course or a course scheduled to be auto-archived before the expiration date set on the pool. Saving a new pool using an archived course shows the message, “Sorry, the course you are trying to create training keys for is archived.” Saving a pool with a start or expiration date that falls after the auto-archive date, shows either the message, “Sorry, the course you are trying to create training keys for is scheduled to be archived before the training key pool start date. Please select another course.”  Or “Sorry, the course you are trying to create training keys for is scheduled to be archived before the training key pool expiration date. Please select another course.”
1. Find Subscriptions – We have added an output option for Price on the Find Subscription search page.
1. Class Roster – We have corrected the negative figure in the Percent complete column on the Class Roster page. The Percent complete column shows the percentage of the required course activities that have been completed by each student. This was displaying a negative number before students started the labs and has been corrected to show zero. 
1. Find Lab Instances – We have updated the Lab Instance details page which was giving a Server Error. From the Find Lab Instances search, a server error displayed when the Details link was selected. LOD removed some legacy exam information which the page previously displayed. Initially, a fix was put in place that incorrectly removed exam results information, this information has been restored.

----------------------------
## Released March 19 2020 

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>

1. Find pages – We have corrected a sorting issue on the Output Options menu. When output options other than the defaults for a page are selected, now when you switch between Sort Alphabetically and Sort by Group, your selections will be retained.
1. Find Classes – We have added an Output Option to the Find Classes page showing the Max Lab RAM per Student showing the highest amount of RAM used in the class’ course per student.
1. Find Enrollments – We have added an Output Option to the Find Enrollments page showing the Job Title field’s data from the User profile.
1. Browse on Demand Catalog – We have updated the Browse on Demand pages to allow multiple Course Tags to be selected by default when users arrive on the page. Along with this, the page can now be set to default either the Match Any or Match All selections on the page. 
1. Class Training Key – We corrected an Application Error which was showing up when you saved after editing a Class Training Key. 
1. Find Lab Instances – We have repositioned the Percent Complete column when the search results are exported from the TMS to match column order on the Find Lab Instances page. 

----------------------------
## Released February 20 2020

### <span style="color:#0078d7;">View Students Progress from the Class Roster</span>

The Class Roster now shows a column for the percentage of course activities completed by each student. This gives an overview of the class’ progress through the lab work and other course activities without going to the individual student enrollments. The column is triggered to display once any student has completed an activity. To be included in the calculation the activity must be required for course completion. Labs, SCORM and LTI modules must be completed to be included while external links, documents, or videos are counted once launched. A numeric percentage shows on the roster while progress bars along with the percentage can be seen on enrollments and course assignments.

### <span style="color:#0078d7;">Cancelling Course Assignments</span>

1. Lab filters for Has Labs or Course Labs now also show results for lab types that do not use RAM like Azure, AWS, or Docker.
1. Find Lab Instances – The Output Option for Exam now shows up when using the print and export links on the Find Lab Instances page.
1. Merge Users – Two user accounts cannot be merged when both students used a training key to enroll into the same class. An assistance message has been added, “We are unable to process this account merge due to multiple enrollments in the same training created by training keys. Please open a Support ticket at https://lods.one/support for assistance.”
1. SCORM video player – SCORM videos played in the Chrome browser encountered a bug that prevented adjusting your place in a video. Players in Chrome can now be adjusted to move forward, to skip ahead, and go back within the video. Seeking in Chrome may take 3-8 seconds to load after moving to a new spot.
1. Class profile – The URL field for the Custom Virtual Classroom class delivery method has increased its capacity from 200 to 500 characters.

----------------------------
## Released February 6 2020

### <span style="color:#0078d7;">Cancelling Course Assignments</span>

We want our Operations Managers to have the ability to cancel course assignments that have been created in error. Course assignments, which are used for self-paced learning, will now have a Course Assignment Status field that is set to either Active or Cancelled. The status defaults to Active when created and is billed for the month when it was created. Operations Managers can change a Course Assignment to the Cancelled status within 24 hours of its creation date/time and only if none of the course activities have been launched. 

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>
1. Achievements – We corrected an issue where Achievements that were set up to be earned multiple times were only being awarded once.
1.  API – Our CreateClass API now passes the instructor into the TMS as the Primary Instructor, and now show in the Find Classes search results Instructor column.
1.  Custom Fields – We have fixed an issue where user role restrictions that applied to editing Custom Fields were incorrectly limiting viewing of the fields for other user roles.
1.  Accessibility updates – Several keyboard focus and navigation updates have been made. Keyboard focus indicator is now visible for:
      - Search buttons on Find pages.
      - The Sort Alphabetically button and Display Times Output Options on the Course Catalog page.
      - The Sign In button in the How Would you Like to Sign In dialog on our Login page.
      - The Send Instructions button on our Forgot Password Login Assistance page.
      - Users can now use the keyboard to navigate to the Edit, Share, and Delete links in the Open and Saved search dialogs on our Find pages.

----------------------------

## Released January 16 2020

### <span style="color:#0078d7;">Reporting Percentage Completed on Labs</span>

Operations Managers and Instructors may display the percentage of work completed in a lab along with the Completion Status on the Find Lab Instances page. Completion Statuses of labs can be, Complete, Cancelled, In Progress, or Error. The percentage of lab completed shows what percent of the lab’s tasks a student completed prior to saving or cancelling, or before the lab errored out. We are awaiting an update from Lab on Demand (LOD) to report the full range of percentages, at this time they are only reporting lab percentages of 0 or 100%.

### <span style="color:#0078d7;">Auto-Archive Date Blocks Class Creation</span>

Class Schedulers and Operations Managers will be prevented from creating classes after a course’s auto-archive date. This is being enforced to support course life cycle planning, allowing course managers to retire courses and labs without conflicting with organizations’ scheduling and students’ lab access. 

When scheduling a class directly in the TMS or through the API, if an auto-archive date is set and any class sessions fall after that date, then the class will not be created. The class import tool checks against the class start date during the upload and will not create classes that start after the auto-archive date. Classes scheduled directly in the TMS or through the API will prevent saving and show an error message, “The course associated with this class is being retired on [Date]. Content will no longer be maintained as of this date. Session dates cannot be scheduled beyond this date. Please consider changing to a newer version of the course; you must change the course or choose different date(s) to save this class.”

### <span style="color:#0078d7;">Auto-Archive Date May Block Saving an Edited Class</span>

For a class that was scheduled prior to setting the associated course’s auto-archive date, Class Schedulers and Operations Managers may edit the class, but will be prevented from saving it if a class session is more than 60 days after the course’s auto-archive date. We want to honor our customers’ training schedules and give you sufficient time to plan and prepare for a change of course content, while still supporting course life cycle planning allowing course managers to retire courses and labs without conflicting with organizations’ scheduling and students’ lab access. 

Updating classes past the archive date through the API will fail and classes edited in the TMS will not be saved. Both will show this error message, “The course associated with this class is scheduled to be archived on [Date]. When editing an existing class, its sessions must fall within 60 days or less after the course auto-archive date. Please consider changing to a newer version of the course; you must change the course or choose different date(s) to save this class.” 

### <span style="color:#0078d7;">TMS Enhancements and Fixes</span>
	
1. Sites – Site profile has had a check box added to turn on or off a Register with Training Key box on customers’ login pages. This functionality speeds up the process for our TMS Coordinator to create standard options for new customers. Sites that already have custom login pages will not be affected by this checkbox field.
1.	Training Keys – Exporting Training Keys was sometimes changing some of the training key values in Excel. The export function for Training Key Pools, Class Enrollment Training Keys, Subscription Training Keys, Class Vouchers, and Event training keys has been corrected to transmit the true key values. 
1.	Class Enrollments – Enrollments created using training keys or the API are now passed to the Customer Portal allowing them to be invoiced to customers.
1.	Courses – When a course creator creates or edits a course adding activities and they exceed the 12-hour expected duration activity limit per day, all activities are retained, but the course is not saved. This allows the course creator to decide how to manage the course; they may increase the course duration and or change the activities.
1.	Course Lab Activities – Some course activities can be set to allow or prevent retakes. The wording displayed for Lab Activities which are set to prevent retakes has been updated to read, “Once you have completed this activity you will not be able to retake it. Do you want to continue?” The message previously read, “Once you have launched this activity you will not be able to retake it.” However, relaunching of the activity is only prevented if the activity has been completed.

----------------------------

## Released December 19 2019

### <span style="color:#0078d7;">Phone Number Added for Instructor Help Desk Support</span>
We want to offer immediate support to instructors teaching a live class. We have set up a direct phone number to our Help Desk for instructor who encounter issues and have questions. Our new Instructor direct support phone number displays on the Class details page; this only shows to the instructor(s) scheduled to teach the class, they can see it before, during, and after class is in session. 

### <span style="color:#0078d7;">Auto Archive Warning Message when Creating or Editing Classes</span>
Class schedulers will receive a warning message when they schedule a class using a course scheduled to be retired. We would like to increase awareness of pending archive dates since labs will not be maintained once the course is retired and after a certain point the labs will become unavailable, which may affect your students’ post class lab access experience.

If the auto archive date is set up and any class session is scheduled to take place on or within 30 days before the auto archive date, the following warning displays when the class is saved, “This course is being retired on [auto archive date and time displayed]. Content will no longer be maintained as of this date. Please consider a newer version.” After clicking OK the class is saved.

The warning displays when creating, editing or cloning a class within 30 days before the auto archive date on the course. Please note the following variances if you are using any of these features:
	
1. Class Import tool: If you are using the class import tool, the warning shows if the start date on a class is within 30 days before the auto-archive date on the course. The import only looks at the start date in the CSV file, it does not calculate dates based on sessions you are scheduling to show a warning.
1. API: No warning will appear for classes created or edited through the API.
1. Class voucher: Warnings or restrictions on scheduling do not apply to classes scheduled using vouchers since they are paid for in advance of redeeming them. 

As a reminder, once a course is archived, the course can no longer be used to create a class or set up self-paced training, however, the labs and course activities still work for students in existing training.

### <span style="color:#0078d7;">Auto Archive Awareness Message on Courses</span>
Class schedulers and Operations managers will see a message highlighted on course profiles when an auto archive date is set. We added this message to increase awareness of approaching archive dates on courses for anyone who can schedule classes; we hope this will assist with your planning and remind you to be looking for a newer version of the course for future classes. 

The awareness message reads, “This course is scheduled to be archived on [auto archive date displayed]. Session dates cannot be scheduled beyond this date. Course content will not be maintained past this date.”

Please note: Once a course is archived, we do not maintain labs or any other course content. Labs may be deactivated on archived courses; it is advisable to find a newer version once a course has been archived.

----------------------------
