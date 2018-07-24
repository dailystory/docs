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

DailyStory supports an unlimited number of campaigns and there is no restriction for how you model you business (e.g. you could create a single campaign or quarterly campaigns). However, the number of campaigns you can have is governed by your license.

> A best practice is to create a campaign for specific activities such as *Black Friday Sales* or *Free Trial*.

## Campaign structure best practices
For lead acquisition campaigns, we recommend creating a campaign called "General Campaign" and then creating specific campaigns for activities you want to track. 

DailyStory will handle assigning leads to the appropriate campaign based on their origination.

### Lead acquisition campaign example
Let's look at a simple example:
	
Your website gets both organic traffic and traffic from a Google Ads campaign "Summer Sales". People complete a Contact Us form on your website and your sales team follows up. 

Now let's add DailyStory.
	
Create a [Magic Form](/acquisition/magic-forms/) in the General Campaign to connect your Contact Us form to DailyStory. Organic visitors that complete the Contact Us form will be added to the General Campaign.

Next, create a "Summer Sales" campaign with [Tracking Links](/link-tracking/) and use those tracking links in your Google Ads.

People that come in through your "Summer Sales" tracking link and complete the Contact Us form will be automatically routed into the "Summer Sales" campaign.

### Email or SMS marketing campaign example
Unlike a lead acquisition campaign where leads are added from forms on your website or through integration with the DailyStory API, an email or SMS marketing campaign doesn't require a catch-all "General Campaign".

Instead you add existing contacts to the campaign, configure the workflow to send the nuturing emails or text messages, and all interactions are related back to that campaign.

## Creating a Campaign
To create a new campaign click the '+ New Campaign' button from the 'All Campaigns' menu option in the navigation. This brings up the Create a New Campaign form:

![Create a Campaign](/articles/campaigns/campaigns-02.png "Create a Campaign")

All that is required to create a campaign is a name.

### Advanced options
You can optionally configure advanced options.

![Advanced options](/articles/campaigns/campaigns-03.png "Advanced options")

* **Assign new leads to** - the account that new leads in this campaign should be assigned to.
* **Workflow behavior** - the default is that any new lead starts at the beginning of the workflow for this campaign. However, this can also be configured so that new leads only receive new workflows. The latter option is useful for newsletter campaigns.
* **Auto-qualify** - leads added to this campaign are automatically marked as qualified.
* **budget** - enables you to configure a cost associated with the campaign.

![Campaign budget](/articles/campaigns/campaigns-04.png "Campaign budget")

> While not enabled in reporting yet, in the future budgeting will allow you to see a cost-per-account or cost-per-lead in reports.

### Editing a Campaign
Campaigns can be edited at anytime. If the campaign is disabled or deleted, the campaign will not run any workflows.

### Deleting a Campaign
To delete a campaign, simply click the Delete button. 

This will immediately disable the campaign. However, the campaign will not be permanently deleted from DailyStory for 10 days.

## Managing a Campaign
Once a campaign is created, or when you view a campaign, you will see different information based on how they campaign is being used.



## Frequently Asked Questions
Below are some frequently asked questions.

### How do I archive a campaign?
To archive a campaign and retain the campaign activity simply mark the campaign as disabled.




A contact can be added to an existing campaign. For example, if you are running a drip campaign to communicate with a new customer, just add the contact to the campaign. 

Each lead is progressed through the campaigns workflow individually. In DailyStory a single contact can be part of multiple campaigns.

> It's important to note that if a campaign had 10 workflow steps it is possible for the campaign's leads to each be at different steps in the campaign's workflow.