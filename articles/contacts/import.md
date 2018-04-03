{
	title: 'Import Contacts',
	description: 'Import contacts into DailyStory'
}
#Import Contacts
Contacts can easily be bulk imported into DailyStory using DailyStory's Bulk Import tool. The only required field to import a contact is an email address.

> The Bulk Import tool can load new contacts from text or from a CSV file.

To find the Bulk Import tool click Accounts > All Contacts:
	
![All Contacts Menu](/articles/contacts/contacts-01.png "All Contacts Menu")

Next, click the + Add contact button:

![Add contact](/articles/contacts/contacts-02.png "Add contact")

Finally, click "bulk import contacts" link on the Create Contact screen:

![Create Contact](/articles/contacts/contacts-03.png "Create Contact")

This will open the Bulk Import tool:
	
![Bulk Import Tool](/articles/contacts/contacts-04.png "Bulk Import Tool")

##Load from text
To load new contacts from a text file simply copy/paste the contact information you wish to import.

Each contact should start on a new line and contacts that contain spaces or commas should be enclosed with double-quotes. 

For example:
	
<code>Amy Jones,amy@example.com,"ACME, Inc."</code> 

After entering the contacts to import click next. On the next screen you can map contacts to fields.

**important:** do not put spaces after comma separated values. Use quotes if content contains a comma.

##Load from CSV
To load new contacts from a CSV (Comma Separated Value) file just click "Select a CSV file to upload". After selecting a file you can map contacts to fields on the next screen.

###How to create a CSV file from Excel
Create a new Excel file or <a href="/articles/contacts/contacts.csv">use our sample CSV file</a>.

> Column headers are optional, but recommeded

Enter data for your contacts that you wish to import.

![Excel](/articles/contacts/excel-01.png "Excel")

Next, save the file locally as a CSV file:
	
![Excel](/articles/contacts/excel-02.png "Excel")

##Map Contact Fields
After selecting the data you are taken to the final screen where you tell DailyStory how to import the contacts:
	
![Map Fields](/articles/contacts/contacts-05.png "Map Fields")

For each data field you will need to either map it to the appropriate field in DailyStory or choose to ignore it. And remember, you **must select an email address** as it is the only required field:
	
![Choose Field](/articles/contacts/contacts-06.png "Choose Field")

For example, we'll map: 
* Fullname to <code>Full name</code>
* Email Address to <code>Email address</code>
* Company to <code>Company or organization name</code>

Next you can optionally select a [campaign](/campaigns) to add the contact to. A contact can be part of one or more campaigns and contact in a campaign is called a lead.

Finally, since the CSV file we imported had headers we'll check "Do not import first row" and then click Import Contacts.

After the contacts are imported we'll see:
	
![Imported](/articles/contacts/contacts-07.png "Imported")

##Important Details to Know About Contact Import
Some important information about contact import:
	
* You can reimport the same contact multiple times. If new information is found, the existing contact will be updated as long as the email addresses are the same.
* When adding contacts to a campaign, new lead notification emails are not sent and if a lead that is of status: <code>Active</code>, <code>Qualified</code>, or <code>Rejected</code> already exists for that contact it will not be re-added.