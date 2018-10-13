{
	title: 'Segments',
	description: 'DailyStory Segment'
}
# Segments
A segment in DailyStory enables you to divide your [contacts](/contacts) into smaller groups designed to enable you to target those groups with narrow campaigns.

DailyStory supports two type of segments: static segments and dynamic segments.

## Static Segments
A static segment is familiar to most marketers - it is a list of contacts you create that meet a specific criteria. Once a segment is created, contacts are easily added to the segment using [search](/search) to narrow the total contacts by properties, such as location. Contacts are then selected and added to one or more static segments.

> A static segment is also created whenver you [import contacts](/contacts/import) to help you quickly find imported contacts.

While static segments are very useful, a more powerful capability of DailyStory is the ability to create dynamic segments that update the contacts within the segment as characteristics of the contacts change.

## Dynamic Segments
The easiest way to think about a dynamic segment is as a search result that is saved. Whenever a dynamic segment is used, the contacts in the segment are updated to match the search results.

Dynamic segment are especially usedful when coupled with [Campaigns](/campaigns) and [User Defined Fields](/contacts/#user-defined-fields). 

### Dynamic Segment Example
As an example, using DailyStory's [MINDBODY integration](/integrations/mindbody) a dynamic segment could be created for Clients that have not visited in the past 30 days. This dynamic segment is then used in a campaign that emails those Clients a series of offers to entice them to return.

> Indexed User Defined Contact fields, which enables those fields to be used in search, are only available to DailyStory Professional and Enterprise customers.

## Creating a Segment
To create a segment navigate to Contacts > New Segment:

![New Segment](/articles/segments/segments-01.png "New Segment")

Add a name, optionally set a description, and click save. Your segment is now ready to use.

> By default, new segments are created as static segments.

You'll now find your segment available in the Segments drop-down when viewing a contact or working with all contacts.

## Add Contacts to a Segment
Once a segment is created you can add contacts to the segment. 

A contact is added individually when viewing a contact. Or, add multiple contacts using DailyStory's Contact Search capabilities to filter contacts.

### Add a Contact
To add a contact to a segment navigate to a contact and use the Segment drop down to select the segment to add the contact to:
	
![Add Contact to Segment](/articles/segments/segments-03.png "Add Contact to Segment")

You can also see a list of all the segments the contact is part of.

### Add Multiple Contacts
To add multiple contats to a segment navigate to contacts. Filter the list of contacts using search, check the contacts you want to add and then select the segment to add them to:
	
![Add Contacts to Segment](/articles/segments/segments-04.png "Add Contacts to Segment")

## Viewing the Contacts in a Segment
To view the contacts in a segment navigate to Segments and select a segment to view:

![View Contacts in Segment](/articles/segments/segments-05.png "View Contacts in Segment")
	
From this view you can also use search to perform some basic searching and filtering of your segment as well as add/remove contacts from your segment.

> Important, if you segment is dynamic you cannot add or remove contacts from your segment. Instead you will need to modify your dynamic segment's search.
	
## Creating Dynamic Segments
To create a dynamic segment, click the Advanced Options link in the Segment editor to access advanced options:
	
![Dynamic Segment](/articles/segments/segments-02.png "Dynamic Segment")

> By default, a new segment is static. You can optionally change your segment to dynamic and add the search criteria used to build the segment.

By selecting the option to make the segment dynamic, you will also need to provide search criteria used to identify contacts.

> Dynamic segments are only available to DailyStory Professional and Enterprise customers.

Next, open a new tab in your browser and navigate to All Contacts. Use [Search](/search) to filter down a list of contacts that meet your specific criteria.

> With dynamic segments it is possible to build dynamic segments that use other segments. For example, all contacts in segment A but not in segment B.

Once you have filtered down your search results, your URL may look similar to:
	
`https://us-1.dailystory.com/Contact?s=apple.com%20campaign:832`

This search looks for all contacts that include the text "apple.com" and are in campaign 832.

Simply copy everything in the URL after the `?`, starting with `s`, and paste that into the Search textbox for your dynamic segment:
	
![Dynamic Segment Search](/articles/segments/segments-06.png "Dynamic Segment Search")	
	
## Deleting a Segment
To delete a segment, edit the segment and simply click the Delete button.

## Segment Permissions
To configure permissions for who can make changes to segments, please see [Understanding Role Permissions](/account/understanding-permissions).