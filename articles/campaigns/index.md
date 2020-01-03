{
	title: 'Campaigns',
	description: 'Campaigns organize related activites and assets'
}
# DailyStory Campaigns
Campaigns organize and manage contacts and assets around activities. Activities include visits to pages, scheduled emails, drip marketing, push notifications and more. 

<iframe src="https://player.vimeo.com/video/382676215" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

> When a [contact](/contacts) is in a campaign it is called a [lead](/leads). A contact may be in multiple campaigns simultaneously.

This guide provides a list of resources to help you get started with Campaigns.

**Create and Edit a Campaign**

* Create a Campaign
* Edit a Campaign
* Add Segments

**Other Topics**

[**Frequently Asked Questions**](#faq)

* Structuring campaigns

## Create a Campaign
To create a campaign, either click the Create Campaign link in the top menu bar or navigate to Campaigns > Campaigns and select + Create from the Campaign's sidebar menu:

![Create a Campaign](/articles/campaigns/campaigns-08.png "Create a Campaign")

The sidebar menu from within Campaigns is also used to create a new campaign: 

![Create a Campaign](/articles/campaigns/campaigns-05.png "Create a Campaign")

Either option opens the Create a Campaign form:

![Create a Campaign](/articles/campaigns/campaigns-02.png "Create a Campaign")

DailyStory supports an unlimited number of campaigns and there is no restriction for how you model your business (e.g. you could create a single campaign or quarterly campaigns). However, the number of campaigns is governed by your license.

> A best practice is to create a campaign for specific activities such as *Black Friday Sales* or *Free Trial*.

On the Create a Campaign screen, there are a number of fields:

* **Name** (required) - The name of the campaign
* **Description** - The description of your campaign within DailyStory.

Other campaign settings:

**Segments**

Add one or more segments used to populate the campaign with existing contacts.

![Segments](/articles/campaigns/campaigns-15.png "Segments")

**Task Assignment**

Assign a follow-up task to a user when a new lead is created in the campaign. Especially useful when running lead collection campaigns, such as from a Popup.

![Task Assignment](/articles/campaigns/campaigns-09.png "Task Assignment")

> Tasks are assigned for leads added through acquisition features such as web forms, popups and the API.

New campaigns are set to "Do no assign a follow-up task".

**Notifications**

Send a notification email to one or more users when a new lead is created.

![New Lead Notifications](/articles/campaigns/campaigns-10.png "New Lead Notifications")

> Notifications are only sent for leads added through acquisition features such as web forms, popups and the API.

New campaigns are set to "Do not send notifications". Unlike Task Assignment, Notifications may be set to send to all users or specific users.

**Duration** 

Set a start/end date for the campaign. Campaigns that are paused will activiate on the start date and campaigns that are active will pause on the end date. 

![Duration](/articles/campaigns/campaigns-11.png "Duration")

> Important - workflows within campaigns will only run during the start/end dates.

New campaigns are set to "Do not set duration".

**Additional Options**

* **Auto qualify leads** - An advanced option used when integrating with a sales CRM, such as Salesforce. New leads are automatically converted to a status of Qualified.
* **Campaign enabled** - Toggle to pause an active campaign. 

![Additional options](/articles/campaigns/campaigns-12.png "Additional options")

New campaigns are set to not auto qualify leads and are enabled.

## Edit a Campaign
To edit a campaign either click on the sidebar menu when viewing a campaign or the more options button to the right of a campaign when viewing a list of campaigns:

![Edit a campaign](/articles/campaigns/campaigns-13.gif "Edit a campaign")

The more options button from the campaign list will also allow editing of a campaign: 

![Edit a campaign](/articles/campaigns/campaigns-14.gif "Edit a campaign")

## Add Segments to a Campaign
When assets, such as [emails](/emails/), are used in your campaign, only those contacts are able to receive messaging from that campaign.

Contacts are added either through lead acquisition or by assigning existing Contacts to the campaign.

While Contacts can be assigned individually to a campaign, assigning segments is the easiest way to add large numbers of contacts efficiently.

And, once segments are assigned to the campaign, you can use the scheduler to control which segments the email (or other asset) will be sent to and when:
	
![Scheduler](/articles/campaigns/campaigns-06.png "Scheduler")

By default the scheduler will send to "Everyone in this campaign". If one or more segments are part of the campaign, you can select to send to those segments as well.	

To add one or more segments to a campaign:

1. Edit the campaign
2. Select one or more segments
3. Save the campaign

For example, the segments "Customer List" and "Digital Agencies":
	
![Add Segments](/articles/campaigns/campaigns-07.png "Add Segments")

> DailyStory takes care of removing duplicate contacts. If a contact is in multiple segments, they are only added to the campaign once. And, if a segment is removed from a campaign, the contact will remain in the campaign if they are part of another segment.


### Lead acquisition campaign example
Let's look at a simple example:
	
Your website gets both organic traffic and traffic from a Google Ads campaign "Summer Sales". People complete a Contact Us form on your website and your sales team follows up. 

Now let's add DailyStory.
	
First, create a [Magic Form](/acquisition/magic-forms/) in the General Campaign to connect your Contact Us form to DailyStory. Organic visitors that complete the Contact Us form are added to the General Campaign.

Next, create a "Summer Sales" campaign with [Tracking Links](/link-tracking/) and use those tracking links in your Google Ads.

People that come in through your "Summer Sales" tracking link and complete the Contact Us form will be automatically routed into the "Summer Sales" campaign.

### Marketing to existing contacts
Unlike a lead acquisition campaign, where leads are added through forms on your website or integration with the DailyStory API, marketing to existing contacts is accomplished by creating a campaign and adding contacts or segments.

[Contacts](/contacts/) are added individually, by selecting multiple contacts from a search result, or by adding segments to the campaign.


## Frequently Asked Questions<a name="faq"></a>
Below are some frequently asked questions about Campaigns.

### What is the recommended campaign structure?
For lead acquisition campaigns, we recommend creating a campaign called "General Campaign" and then creating specific campaigns for activities you want to track. 

DailyStory will handle assigning leads to the appropriate campaign based on their origination.

### What happens when I delete a campaign?
When a campaign is deleted it is moved to the Trash and the campaign, assets and workflows are disabled. However, the campaign will not be permanently deleted and is recoverable from the Trash for up to 7 days. After 7 days the campaign is permanently deleted.

Once the campaign is deleted all assets associated with the campaign will be tagged as "Unassigned".

### Why don't I see my campaign when trying to assign it to an asset?
In order for a campaign to be avaiable to assign assets, it must be Active. Double check that you have enabled the campaign in the campaign settings.

### What is an "Unassigned" campaign?
In your use of DailyStory you may see an email or other campaign asset associated with the campaign "Unassigned". 

The "Unassigned" campaign is a special type of campaign used when an asset is no longer associated with a campaign. 

### How do I archive a campaign?
To archive a campaign and retain the campaign activity mark the campaign as disabled. Archiving a campaign retains all the data and assets for reporting purposes, but disables workflows and other campaign automations.

### What happens when a contact is added to a campaign?
When a contact is added to a campaign either directly or as part of a segment, a new ["Lead"](/leads/) is created for that contact in the campaign. 

Next, if the campaign has an associated workflow, the lead is run through the workflow. The lead is also eligible to receive any assets scheduled for the campaign (emails, text messages, push notifications, etc.). And, if the campaign has automations or scoring rules in place, those are run too.