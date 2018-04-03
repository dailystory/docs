{
	title: 'Profile Data Import',
	description: 'How to import profile data into a DailyStory lead'
}
# How to import profile data into a DailyStory lead
DailyStory makes it easy to import additional data that can be associated with a lead. Once imported you can create rules and automations and use the data for personalization in emails, landing pages, and text messages.

> For example, after running a webinar export data such as who attended, who asked questions, who participated in polls. Next import that into the leads in DailyStory and setup campaigns based on webinar participation.

## Create and manage profile fields
Before you can import data into a DailyStory lead profile you first need to create the profile fields.

> Creating the profile fields enables DailyStory to know how to store and later access your data. 

<ol class="step"><li value="1">Open a campaign</li></ol>
Navigate to the Leads or Contacts section of an existing campaign. From the action button, select Manage Profile Fields:
	
![Manage Profile Fields](/articles/leads/import-profiles-01.png "Manage Profile Fields")

This opens up the Manage Lead Profiles Fields page:
	
![Manage Lead Profile Fields page](/articles/leads/import-profiles-02.png "Manage Lead Profile Fields page")

The Manage Lead Profile Fields page enables you to add or delete profile fields. You must create profile fields	that correspond to the data you want to import.

For example, if the imported data contains webinar participation data you may want to create a field to identify if the lead attended the webinar (as shown in the screen shot above).
<ol class="step"><li value="2">Create profile fields</li></ol>
All that is required it to enter the name of the profile field. If the name conflicts with an existing field you will receive an error, otherwise the new profile field will be created.

DailyStory automatically generates an API name for your profile field. The API name is used for personalization in emails, landing pages, and text messages.	

<ol class="step"><li value="3">Import data</li></ol>
After creating the fields, you are ready to import the data.

## Import profile field data
To import profile data either click the + Import Profile Data button on the Manage Lead Profile Fields page discussed above.

> The imported profile data must contain an email address to identify which lead the data applies to.

You can also select Import Profile Data from the drop down button on the Leads or Contacts page within a campaign.

![Import Profile Data](/articles/leads/import-profiles-03.png "Manage Profile Data")

> The Profile Data Import tool can load new profile data from text or from a CSV file.

![Import Tool](/articles/leads/import-profiles-04.png "Import Tool")

### Load from text
To load profile data from a text file simply copy/paste the profile data you wish to import.

Each record should start on a new line and data that contain spaces or commas should be enclosed with double-quotes. 

For example:
	
<code>amy@example.com,"Great webinar!",Yes,3</code> 

After entering the profile data to import click next. On the next screen you can map profile fields to the imported data.

**important:** do not put spaces after comma separated values. Use quotes if content contains a comma.

### Load from CSV
To load profile data from a CSV (Comma Separated Value) file just click "Select a CSV file to upload". After selecting a file you are sent to the next screen where you can map profile fields to the imported data..

#### How to create a CSV file from Excel
Create a new Excel file or <a href="/articles/leads/sample-profile-data.csv">use our sample CSV file</a>.

> Column headers are optional, but recommeded

Enter data for your contacts that you wish to import.

![Excel](/articles/leads/excel-01.png "Excel")

Next, save the file locally as a CSV file:
	
![Excel](/articles/contacts/excel-02.png "Excel")

##Map Profile Fields
After selecting the data you are taken to the final screen where you tell DailyStory which profile fields to map the imported data to:
	
![Map Fields](/articles/leads/import-profile-05.png "Map Fields")

For each data field you will need to map it to the appropriate field in DailyStory or choose to ignore it. And remember, you **must select an email address** as it is the only required field:
	
![Choose Field](/articles/contacts/contacts-06.png "Choose Field")

For example, we'll map: 
* Attended to <code>attended webinar</code>
* Email Address to <code>Email address</code>

Finally, since the CSV file we imported had headers we'll check "Do not import first row" and then click Import Profile Data.

The import process is started and can taken several minutes depending upon how much data is being imported.

### Important Details to Know about Profile Data Import
Some important information about importing profile data:
	
* If a lead already has a value for the data being imported, the previous value will be replaced with the new value.