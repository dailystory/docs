---
layout: _ArticleLayout
title: Campaigns
description: Campaigns are the cornerstone of DailyStory
---
#Campaigns
Campaigns are the cornerstone of DailyStory - everything in DailyStory first starts with a campaign. 

[Contacts](/contacts) are assigned to campaigns as leads. All capabilities around reporting,and account activity are associated with a campaign.

![Campaigns](/articles/campaigns/campaigns-01.png "Campaigns")

DailyStory supports an unlimited number of campaigns and there is no restriction for how you model you business (e.g. you could create a single campaign or quarterly campaigns). 

> A best practice is to create a campaign for specific activities such as *Black Friday Sales* or *Free Trial*.

You do not need to recreate campaigns to add new leads to your campaign. For example, if you are running a drip campaign to communicate with a new customer just add the contact to the campaign. Contacts within a campaign are called leads and each lead is progressed through the campaigns workflow individually.

> If a campaign had 10 workflow steps it is possible for leads to be at different steps in the workflow.

## Creating a Campaign
To create a new campaign click the '+ New Campaign' button from the 'All Campaigns' menu option in the navigation. This brings up the Create a New Campaign form:

![Create a Campaign](/articles/campaigns/campaigns-02.png "Create a Campaign")

All that is required to create a basic campaign is a campaign name and description.

Next, you can select the type of campaign to create. Currently only two types are supported and the selected campaign only impacts the reports on the campaign home page. By default new campaigns are automatically set to **Lead generation**:

![Campaign type](/articles/campaigns/campaigns-03.png "Campaign type")
	
* Lead generation - a lead generation campaign will display reports and forecasts for leads added to your campaign through web forms or the API.
* Email campaign - an email campaign displays reports about email delivery, bounces, link clicks, and more.

You can then select who **new leads are assigned to**. This selection list will contain a list of all the users that have accounts for your DailyStory account.

The **budget** enables you to configure a cost associated with the campaign.

![Campaign budget](/articles/campaigns/campaigns-04.png "Campaign budget")

> While not enabled in reporting yet, budgeting will allow you to see a cost-per-account or cost-per-lead in reports.

The **campaign enabled** switch enables you to control whether or not a campaign is active and enabled. Campaigns that are disabled are not available as a choice when creating new assets, such as emails.

![Campaign enabled](/articles/campaigns/campaigns-05.png "Campaign enabled")

## Editing a Campaign
Campaigns can be edited at anytime and changes will not impact running campaigns unless the campaign is marked as disabled. If the campaign is marked as disabled, the campaign will effectively be paused and campaign workflows will not be run.

## Deleting a Campaign
To delete a campaign, first edit the campaign then click the Delete button. This will immediately disable the campaign. However, the campaign will not be completely deleted from DailyStory for 10 days.