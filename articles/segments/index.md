{
	title: 'Segments',
	description: 'DailyStory Segment'
}
# DailyStory Segments
A segment in DailyStory enables you to organize your [contacts](/contacts) into smaller groups. This enables you to target those groups with specific messages using the most appropriate channel.

This guide provides a list of resources to help you get started with Segments.

**Create and Edit a Segment**

* [Create a Segment](#create-a-segment)
* [Edit a Segment](#edit-a-segment)
* [Create a Dynamic Segment](#create-a-dynamic-segment)
* [Types of Segments](#types-of-segments)
* [Create a dynamic segment from search](#create-a-dynamic-segment-from-search)

**Segment Management**

* [View Contacts in a Segment](#viewing-the-contacts-in-a-segment)
* [Add Contacts to a Segment](#add-contacts-to-a-segment)
* [Restrict access through permissions](#restricting-access-through-permissions)

**Frequently Asked Questions**

* [What is a static segment?](#what-is-a-static-segment)
* [What is a dynamic segment?](#what-is-a-dynamic-segment)
* [How often are dynamic segments updated?](#how-often-are-dynamic-segments-updated)
* [Why do some contacts not show up in my segment?](#why-do-some-contacts-not-show-up-in-my-segment)
* [How do I remove contacts from a Dynamic segment?](#how-do-i-remove-contacts-from-a-dynamic-segment)
* [How do I use segments in a campaign?](#how-do-i-use-segments-in-a-campaign)
* [How do I send a message to a specific segment?](#how-do-i-send-a-message-to-a-specific-segment)

## Create a Segment
To create a segment, either: 

* Navigate to Contacts > New Segment. 
* Navigate to Contacts > All Segments and click `+ Create` in the Segment menu.
* Use the [Create Segment button](#create-a-dynamic-segment-from-search) from a list of search results
* [Import a list of Contacts](/contacts/import)

With the exception of creating a segment from import, all other options will open the Create Segment Editor.

![New Segment](/articles/segments/segments-01.png "New Segment")

To finish creating a segment add a name, optionally set a description, and click save. Your segment is now ready to use.

> By default, new segments are created as [static segments](#static-segments).

The newly created segment is now available in the Edit Campaign screen, segments drop-down when viewing a contact, and when viewing a list of contacts.

## Edit a Segment
To edit a segment navigate to Contacts > All Segments. Here you will see a list of all the active segments. Click on the name of the segment or use the quick menu on the right to Edit the Segment.

![All Segments](/articles/segments/segments-07.png "All Segments")

The Edit Segment screen will open and is nearly identical to the Create Segment screen.

## Add Contacts to a Segment
Once a segment is created you can add contacts to the segment. 

> You can only add contacts to a [static segment](#static-segments). If you try to add a contact to a [dynamic segment](#dynamic-segments) you will be unable to do so.

### Add a Single Contact
A contact is added individually when viewing a list of Contacts. 

![Add Contact](/articles/segments/segments-08.gif "Add Contact")

### Add Multiple Contacts
Add multiple contacts to a segment using DailyStory's Contact Search capabilities. Filter a list of contacts and check the contacts you wish to add to your segment.

![Add Contacts to Segment](/articles/segments/segments-04.png "Add Contacts to Segment")

### Add from Contact Detail
You can also add a contact to a segment when viewing a contact record. Navigate to a contact and use the Segment drop down to select the segment to add the contact to.
	
![Add Contact to Segment](/articles/segments/segments-03.png "Add Contact to Segment")

From this screen you can also see a list of all the segments this contact is in.

## Viewing the Contacts in a Segment
To view the contacts in a segment navigate to Segments and select a segment to view:

![View Contacts in Segment](/articles/segments/segments-05.png "View Contacts in Segment")
	
From this view you can also use search to perform some basic searching and filtering of segment's Contacts as well as add/remove contacts from your segment.

> Important, if you segment is dynamic you cannot add or remove contacts from your segment. Instead you will need to modify the search criteria of the dynamic segment.

## Types of Segments
DailyStory supports two type of segments: static segments and dynamic segments.

### Static Segments
A static segment is familiar to most marketers: a list of contacts you create that meet a specific criteria. 

Once a segment is created, contacts are easily added to the segment using [search](/search) to narrow the total contacts by properties, such as location. Contacts are then selected and added to one or more static segments.

> A static segment is also created whenver you [import contacts](/contacts/import) to help you quickly find imported contacts.

While static segments are very useful, a more powerful capability of DailyStory is the ability to create dynamic segments. 

Dynamic Segments update the contacts within the segment as characteristics of the contacts change. For example, if the Dynamic Segment was based on `Eligibility Date` each day new Contacts may become eligible and fit the requirements of the Dynamic Segment's search.

### Dynamic Segments
The easiest way to think about a dynamic segment is as a search result that is saved. Whenever a Dynamic Segment is used, the contacts in the segment are updated to match the search results.

Dynamic segment are especially usedful when coupled with [Campaigns](/campaigns) and [User Defined Fields](/contacts/#user-defined-fields). 

<iframe src="https://player.vimeo.com/video/313256117" width="640" height="480" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

### Dynamic Segment Example
As an example, using DailyStory's [MINDBODY integration](/integrations/mindbody) a dynamic segment could be created for Clients that have not visited in the past 30 days. This dynamic segment is then used in a campaign that emails those Clients a series of offers to entice them to return.

> Indexed User Defined Contact fields, which enables those fields to be used in search, are only available to DailyStory Professional and Enterprise customers.
	
## Create a Dynamic Segment
To create a dynamic segment, create a new segment. Next, scroll down to `Configure the type of segment` and select Dynamic Segment.

![Dynamic Segment](/articles/segments/segments-02.gif "Dynamic Segment")

> By default, new segments are static and Dynamic Segments are only available to DailyStory Professional and Enterprise customers.

By selecting the option to make the segment dynamic, you will also need to provide search criteria used to identify contacts.

Search criteria for a Dynamic Segment starts with `s=`. For example, to find everyone with the domain `example.com` the search criteria is: `s=example.com`.

The Dynamic Search criteria follows the same format as Contact search. But typing this in is tedious. It's much, much easier to create a Dynamic Segment from search.

### Create a Dynamic Segment from Search
The easiest was to create a Dynamic Segment is to start in Contact search. Simply search using either basic or advanced search to find a list of contacts.

> With dynamic segments it is possible to build dynamic segments that use other segments. For example, all contacts in segment A but not in segment B.

Once you have filtered down your search results, your URL may look similar to:
	
`https://us-1.dailystory.com/Contact?s=apple.com%20campaign:832`

This search looks for all contacts that include the text "apple.com" and are in campaign 832. 

Scroll to the bottom of the Contact search page and you'll find the `Create Segment` button. 

![Create Segment Button](/articles/segments/segments-09.png "Create Segment Button")	

Click this button and you will be taken to the Create a Segment screen. The segment will automatically be set to Dynamic and the search results from your Contact's search query will appear in the Segment's search box:

![Dynamic Segment Search](/articles/segments/segments-06.png "Dynamic Segment Search")	
	
## Deleting a Segment
To delete a segment, edit the segment and simply click the Delete button.

When a segment is deleted it is inactive and not accessible for adding/removing contacts, adding to campaigns or dynamically updating.

After 5 days any Segments in the Trash are automatically deleted.

## Restricting access through permissions
To configure permissions for who can make changes to segments, please see [Understanding Role Permissions](/account/understanding-permissions).

## Frequently Asked Questions
Below are some frequently asked questions about Segments.

### What is a static segment?
A static segment is a segment that you manually add/remove Contacts to.

### What is a dynamic segment?
A dynamic segment is a segment that is automatically built from the results of a search. Contacts cannot be added/removed as only contacts that match the search are part of the segment.

### How often are dynamic segments updated?
Dynamic segments are rebuilt - where contacts are added or removed by DailyStory every 24 hours at 2AM in the timezone where the DailyStory data center is located. And, anytime a dynamic segment is saved it is also rebuilt.

### Why do some contacts not show up in my segment?
Contacts may not show up in your segment for several reasons. First, they may not have been added, may have been recently removed, or do not match the search criteria for the dynamic segment. If a contact is inactive or has opted out of all channels (do not contact) they also will not show up in the segment.

### How do I remove contacts from a Dynamic segment?
The only way to remove contacts from a dynamic segment is to build a search that excludes them.

### How do I use segments in a campaign?
To add a segment to a campaign, so that it is available in the scheduler for emails, push notifications, text messages, etc. you need to edit the campaign and add the segments.

### How do I send a message to a specific segment?
To send a message, such as an email, to a specific segment edit the email in the campaign and use the scheduler. The scheduler provides an option for who to send to. Here you can pick the segments to send your message to.