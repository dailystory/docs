{
	title: 'Campaigns',
	description: 'Campaigns organize related activites and assets'
}
# DailyStory Campaigns
Campaigns are a cornerstone feature of DailyStory. Campaigns organize related activites and assets. 

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FVxbtl_DHzbA%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DVxbtl_DHzbA&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FVxbtl_DHzbA%2Fhqdefault.jpg&key=internal&type=text%2Fhtml&schema=youtube" width="500" height="281" scrolling="no" frameborder="0" allowfullscreen></iframe>

> [Contacts](/contacts) are assigned to campaigns. When a contact is in a campaign it is called a [lead](/leads). A contact can be in multiple campaigns simultaneously.

All reporting and account activity is associated with a campaign.

![Campaigns](/articles/campaigns/campaigns-01.png "Campaigns")

DailyStory supports an unlimited number of campaigns and there is no restriction for how you model your business (e.g. you could create a single campaign or quarterly campaigns). However, the number of campaigns is governed by your license.

> A best practice is to create a campaign for specific activities such as *Black Friday Sales* or *Free Trial*.

## Campaign structure best practices
For lead acquisition campaigns, we recommend creating a campaign called "General Campaign" and then creating specific campaigns for activities you want to track. 

DailyStory will handle assigning leads to the appropriate campaign based on their origination.

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

## Creating a Campaign
To create a new campaign click the '+ Create' link in the sidebar. 

![Create a Campaign](/articles/campaigns/campaigns-05.png "Create a Campaign")

This brings up the Create a Campaign form:

![Create a Campaign](/articles/campaigns/campaigns-02.png "Create a Campaign")

Only the name is required to create the campaign. Use the description to provide helpful information about your campaign.

### Add Segments to a Campaign
When assets, such as [emails](/emails/), are created for your campaign, the available contacts to send the asset to are determined by the segments that are part of the campaign.  Once segments are assigned to the campaign, you can use the scheduler to control which segments the email (or other asset) will be sent to and when:
	
![Scheduler](/articles/campaigns/campaigns-06.png "Scheduler")

By default the scheduler will send to "Everyone in this campaign". If one or more segments are part of the campaign, you can select to send to those segments as well.	

To add one or more segments to a campaign:

1. Edit the campaign
2. Select one or more segments
3. Save the campaign

For example, the segments "Customer List" and "Digital Agencies":
	
![Add Segments](/articles/campaigns/campaigns-07.png "Add Segments")

You may also choose to exclude certain segments as well.  This option will always allow you to choose ANY segment that has been created, not just those assigned to the campaign.

> Note, DailyStory takes care of removing duplicates. If a contact is in multiple segments, they will only be added to your campaign once. And, if a segment is removed from a campaign, the contact will remain in the campaign if they are part of another segment.

### Additional Options
* **Assign new leads to** - Lead assignment enables you to assign leads to a member of your team.
* **Auto-qualify** - Leads added to this campaign are automatically marked as qualified.

### Editing a Campaign
Campaigns can be edited at any time to change name, description or other details. Segments may also be added or removed. 

Note: deleting or pausing a campaign will prevent workflow, scheduled activites, rules and automations and other campaign activites from processing. 

## Frequently Asked Questions

### What happens when I delete a campaign?
When a campaign is deleted it is moved to the Trash and the campaign is disabled. However, the campaign will not be permanently deleted and can be recovered from the Trash. Once the campaign is deleted all assets associated with the campaign will be tagged as "Unassigned" and when edited may be assigned to another campaign.

### Why don't I see my campaign when trying to assign it to an asset?
In order for a campaign to be avaiable to assign assets, it must first be enabled.  Double check that you have enabled the campaign in the campaign settings.

### What is an "Unassigned" campaign?
In your use of DailyStory you may see an email or other campaign asset associated with the campaign "Unassigned". The "Unassigned" campaign is a special type of campaign used when an asset is no longer associated with a campaign. An "Unassigned" asset can be associated with a campaign by editing it. When opened a popup will appear asking which campaign the asset should be part of. 

### How do I archive a campaign?
To archive a campaign and retain the campaign activity mark the campaign as disabled. While archived campaigns are not active, archiving a campaign retains all the data and assets for reporting purposes.

### What happens when a contact is added to a campaign?
When a contact is added to a campaign either directly or as part of a segment, a new ["Lead"](/leads/) is created for that contact in the campaign. Next, if the campaign has an associated workflow, the lead is run through the workflow. The lead is also eligible to receive any assets scheduled for the campaign (emails, text messages, push notifications, etc.). And, if the campaign has automations or scoring rules in place, those will also be run on the lead.
 
## Warning messages

### No one to send to - add contacts or segments to your campaign<a name="warning-scheduler-1"></a>
This warning message indicates that no segments or contacts are used in the [campaign](https://docs.dailystory.com/campaigns/). The message may still be scheduled and segments/contacts can be added later. To resolve, either:

* Edit the campaign and add segments
* Select individual contacts to add to the campaign