<img src = "ecf.jpg" height = "165" width = "330"/>

# ECF
## IT Dashboard Developer Internship
###### James McElduff
###### Summer 2017

#### Tasklist
- [ ] Qlikview to Qliksense migration
  - [x] Rate Plan Surveillance
  - [ ] Support Center
- [ ] New dashboards for Qliksense
- [ ] Documentation for Qlik Knowledge Base
- [ ] Visual enhancements
- [ ] Improve existing dashboards

#### Knowledge List
- [ ] HTML, Javascript, CSS
- [x] SQL/T-SQL
- [ ] Markdown
- [ ] Qliksense/Qlikview data expressions
- [ ] Qlikscript

### Calendar
## Week of May 22 - May 26, 2017
1. Monday: Onboarding with HR, Nareen, getting settled on my first day.
2. Tuesday: Learning the basics of Qlik, completing training.
3. Wednesday: Continuing with the Qliksense textbook, more company training. Learned about SQL/T-SQL. Practiced with Qliksense dashboards.
4. Thursday: Finished training and Qliksense textbook, learned more about SQL/T-SQL from Donn.
5. Friday: 3pm dismissal because of Memorial Day Weekend. Practiced with Qliksense dashboards from examples found online.
#### Weekly Summary: First week, can't expect (or be expected) much. Learned quickly how to use Qliksense, SQL/T-SQL.

## Week of May 29 - June 2, 2017
1. Monday: Memorial Day, no work.
2. Tuesday: Waiting to be granted permissions to databases and have Qlikview installed so I can begin my first small project of a Qlikview to Qliksense migration. Practicing with Markdown and the capabilities (and limits) of the file type. Worked on the Equity Example (data from Qliksense online forums), sharpened up visuals and attempted to further understand expressions. Attended a Qliksense NPrinting meeting to talk about Qlik licenses and problems. Became involved with NPrinting Testing.
3. Wednesday: The battle for permissions wages on. Qlik NPrinting meeting to set up Qliksense to email out to people (my understanding). Needed to obtain permission to install Qlik NPrinting, obtain permission to access the report files, obtain access to the NPrinting amin privileges. NPrinting meeting to set up Qliksense subscription reports - found out I don't have enough permissions to do anything. Worked to compile docmentation for NPrinting subscription reports obtained from Doug. Important items for each report include dashboard name, NSQ file, recipients, report name, filters (name, field name, field value), and schedule. Create a table in Excel as a preliminary answer to the documentation. Will be eventually converted and added to documentation for all server actions.
4. Thursday: QlikView has been installed. Reading "Simply SQL" to better learn SQL. Tasked to migrate the Rate Plan Surveillance Dashboad from QlikView to QlikSense. Copied script from QlikView to Qliksense. Migrated the Overview page and most of the Assignment Audit page (just the pivot table left) of the Rate Plan Surveillance Dashboard to a QlikSense App.
5. Friday: Finished the pivot table addition. Trying to figure out hot to make it look nicer - so it shows the full cells first, instead of "-". Also researching if having an image inside of a table is even possible in QlikSense. Also migrated the "Raw Data Check" page to QlikSense. Finished the migration of "Rate Plan Surveillance" from QlikView to QliKSense. Images in tables isn't yet available to QlikSense so I had to use ASCII characters of a circle, and change the color (green/red) based on validation requirements. Sorting on the pivot table in the "Assignment Audit" page is not perfect, need to figure that out with Donn (figured it out - uncheck "Allow Null Values" for each dimension. Attended a 2hr New Hire Orientation Meeting. Began reading documentation for QDF (Qlik Deployment Framework): the file folders in a Qlik App.
#### Weekly Summary: Lots of waiting for permissions. Began/finished the "Rate Plan Surveillance" migration example from QlikView to QlikSense. Learned more about SQL and NPrinting.

## Week of June 5 - June 9, 2017
1. Monday: Visual edits on the Rate Plan Surveillance Dashboard per Donn's recommendations. Learned more about QDF and how it creates an organized folder structure for each QlikSense application. This is used to better document and keep track of our work. Attended a Lunch & Learn with Joe Inferrera who spoke broadly of the organization/company. Met the other interns.
2. Tuesday: Began the day by learning more about the QDF and working through the practice examples.
3. Wednesday: Started to migrate "Support Center" over to QlikSense. Received permissions to open files. Working on QlikSense Desktop, will upload to web later - need to learn how to connect to SQL DB (how to find it in the QlikView script).
4. Finished the migration for the Support Center dashboard on QlikSense Desktop. Need to upload it to the server to add things like climber selection panels and heat maps (no extension on my local QlikSense Desktop) in order to finish the dashboard. Need a license/subscription to QlikView to continue opening QlikView files. Also need to secure connection to SupportCenter DB to get data flowing.
5. Friday: Continued to work on the Support Center dashboard migration. Figuerd out the QVD Generator and connected the proper path for the Support Center Dashboard. Working on heatmap and climber filter visualizations. Calendar heatmap extension will not work because we need a 2 dimensional heatmap, and the calendar extension is monodimensional. Working to clean up and simplify the logic in the Support Center. Will work to remove the QVD aspect of it, as it does not get a lot of data from the DB. Working to let the scatter chart's dimension depend upon a filter pane. Also trying to clean up the date selection process, and remove the "Internal Engine Error" error. It has something to do with the variables and picking a singular day.
#### Weekly Summary: Started the Support Center Dashboard migration. Learned about QDF.

## Week of June 12 - June 16, 2017
1. Monday: Working on completing the Support Center Dashboard. Repositioned items and cleaned up UI - instead of climber selections, using straight filters (built in) that work with less speed bumps, cleaned up format of 2d heatmap. Figured out the cyclic dimensions in Qlik Sense. Built a "Dimension Selector" INLINE in the Data Load Editor with all of the dimension names that I want to cycle through. Then the dimension for the scatter chart (that I want the user to be able to cycle through different dimensions) gets the selection from "Dimension Selector" by using `=[$(=MinString(Selector)))]` which gets the selected dimension's data. So the scatter chart is controlled by the selector filter above it. One problem is that one dimension does not take kindly to the "color by dimension" option, which is still to be figured out. The "Open Requests" line chart also declares an "Internal Engine Error" when selecting individual days, I suspect because of `SupportRequestStatusName={'Open', 'Assigned'}` - having two optoins for SupportRequestStatusName, as that is the only difference from the other line graphs. Finished the Support Center Dashboard, still to do: clean up/streamline data loading.
2. Tuesday: Time towards cleaning up data model - is the SubRequests table needed?
