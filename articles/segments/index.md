{
	title: 'Segments',
	description: 'DailyStory Segment'
}
# Segments
A segment in DailyStory enables you to divide your [contacts](/contacts) into smaller groups designed to enable you to target those groups with narrow campaigns.

A segment is created by using [search](/search) to narrow the total contacts by properties, such as location. The created segment can be static or dynamic. A static segment has a fixed set of contacts whereas a dynamic segment is updated as contacts either match or do not match the segment filters.

> DailyStory Enterprise customers have the ablity to create segments filtered on custom properties.

# Creating a Segment
To create a segment navigate to Contacts > New Segment:

![New Segment](/articles/segments/segments-01.png "New Segment")

Add a name, optionally set a description, and click save. Your segment is now ready to use.

## Advanced Segment Options
Click the Advanced Options link in the Segment editor to access advanced options.

By default, your segment is configured as static. You can optionally change your segment to dynamic and add the search criteria used to build the segment.

When set to dynamic, the contacts that fit the segment's criteria can change as information about those contacts change.

> Dynamic segments are only available to DailyStory Premium and Enterprise customers.

# Add Contacts to a Segment
Once a segment is created you can add contacts to the segment. 

A contact is added individually when viewing a contact. Or, add multiple contacts using DailyStory's Contact Search capabilities to filter contacts.

## Add a Contact

## Add Multiple Contacts

### Changing a Lead's Status
A lead's status can be changed manually and automatically.

> By default, all newly added leads start as Active.

#### Manually Changing a Lead's Status
When viewing a lead, use the Reject or Qualified buttons to change a lead's status:
	
![Lead Buttons](/articles/leads/leads-01.png "Lead Buttons")

To delete leads from a campaign either view All Leads or Leads within a campaign placing a check to all the leads you want to delete:

![Lead Bulk Edit](/articles/leads/leads-02.png "Lead Bulk Edit")

Click Remove from campaign and those leads are marked as deleted.

#### Automatically Changing a Lead's Status
A lead's status can be changed automatically in a few ways. For example, if a [contact's status](/contacts) is changed to Inactive or Bounced all of the leads for that contact are automatically marked as Rejected. Similarly, if the contact's status is changed to Deleted all of the leads for that contact are automatically marked as Deleted too.

In addition to these built-in rules, you can also utilize [campaign automation](/campaigns) to change a lead's status based on conditions you define.

For example, if the lead accumulates points through scoring, visits certain pages in your website, has a specific email address and so on you can change a lead's status using the campaign's automation:

![Automate Qualification](/articles/leads/leads-03.png "Automate Qualification")

Similarly, if a lead has negative attributes, such as a competitor's email address or hasn't been active in a period of time, you can automatically reject the lead:
	
![Automate Disqualification](/articles/leads/leads-04.png "Automate Disqualification")

Automation rules give you the flexibility to control how DailyStory manages your leads based on your specific business conditions.	

### Salesforce Integration
WIth [Salesforce integration](/integrations/salesforce) a lead that is qualified is pushed into Salesforce and tracked through opportunity won/loss. 

If the Salesforce opportunity because won or lost, that status is tracked back into DailyStory and revenue associated with the won opportunity is reflected in the campaign.

> This powerful integration allows you to see which of your campaigns contributed revenue to your business.