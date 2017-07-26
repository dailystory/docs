---
layout: _ArticleLayout
title: Leads
description: DailyStory Lead
---
# Lead
A lead in DailyStory represents a [contact](/contacts) that is part of a [campaign](/campaigns). A contact can be part of no campaigns or many campaigns. When a contact is in a campaign it is called a lead.

> For example, if a customer is part of a renewal campaign, but has also downloaded a white paper and signed up for a newsletter there is a single contact and three leads (presuming 3 campaigns: renewal, newsletter and white paper).

# Lead Status
Each lead has a status that corresponds to the leads state within the campaign:

* Active - the default state of new leads
* Qualified - leads that considered successful and no longer Active.
* Rejected - leads that considered unsuccessful and no longer Active.
* Duplicate - leads that are duplicates of an existing lead and still Active.
* Deleted - leads that are considered invalid and are no longer Active.

> The status of the lead determines if they are available for workflow, automation and rules within a campaign.

### Workflow, Scoring and Automation
Leads that are Active or Duplicate are processed through workflows, scoring and automation. Leads that are Qualified, Rejected or Deleted are no longer processed through workflows, scoring and automation.

### Changing a Lead's Status
A lead's status can be changed manually and automatically.

> By default, all newly added leads start as Active.

#### Manually Changing a Lead's Status
When viewing a lead, use the Reject or Qualifed buttons to change a lead's status:
	
![Lead Buttons](/articles/leads/leads-01.png "Lead Buttons")

To delete leads from a campaign either view All Leads or Leads within a campaign placing a check to all the leads you want to delete:

![Lead Bulk Edit](/articles/leads/leads-02.png "Lead Bulk Edit")

Click Remove from capaign and those leads are marked as deleted.

#### Automatically Changing a Lead's Status
A lead's status can be changed automatically in a few ways. For example, if a [contact's status](/contacts) is changed to Inactive or Bounced all of the leads for that contact are automatically marked as Rejected. Similarlly, if the contact's status is changed to Deleted all of the leads for that contact are automatically marked as Deleted too.

In addition to these buit-in rules, you can also utilize [campaign automation](/campaigns) to change a lead's status based on conditions you define.

For example, if the lead accumulate's points through scoring, visits certain pages in your website, has a specific email address and so on you can change a lead's status:

![Automate Qualification](/articles/leads/leads-03.png "Automate Qualification")

Similarlly, if a lead has negative attributes, such as a competitor's email address or hasn't been active in a period of time, you can automatically reject the lead:
	
![Automate Disqualification](/articles/leads/leads-04.png "Automate Disqualification")

Automation rules give you flexibility to control how DailyStory manages your leads based on your specific business conditions.	

### Salesforce Integration
WIth [Salesforce integration](/integrations/salesforce) a lead that is qualified is pushed into Salesforce and tracked through opportunity won/loss. 

If the Salesforce opportunity because won or lost, that status is tracked back into DailyStory and revenue associated with the won opportunity is reflected in the campaign.

> This powerful integration allows you to see which of your campaigns contributed revenue to your business.