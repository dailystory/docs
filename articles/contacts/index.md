{
title: 'Contacts',
description: 'A DailyStory Contact is a customer or prospective customer managed by DailyStory.'
}
#Contacts
A DailyStory Contact is a customer or prospective customer managed by DailyStory. 

While there is only a single contact for an individual managed by DailyStory, the contact may be part of multiple campaigns. For example, a contact can be subscribed to a newsletter, part of a nurturing drip campaign, and part of a new membership email sequence.

A [lead](/leads) represents the contact within a specific campaign. When viewing a contact you can see the campaigns that contact is part of.

##All Contacts
To view all of your contacts click Contacts > All Contacts. You will be presented with a list all contacts.

![All Contacts](/articles/contacts/contacts-08.png "All Contacts")

From All Contacts you can select contacts and add them to a Campaign or Segment.

![Add Contacts to a Campaign](/articles/contacts/contacts-09.png "Add Contacts to a Campaign")

Going through a list of contacts one-by-one to add them to your campaigns or segments is slow. Instead, you can filter the contacts shown using search.

###Searching and Filtering All Contacts
To quickly search your contacts you can type any text into the quick search text box. 

This will search across all contact fields and return any matches. For example, if you search for "Dallas" it may return people who's first name is Dallas and people who live in the city Dallas.

![Quick Search](/articles/contacts/contacts-10.png "Quick Search")

While useful, sometimes you want to get more specific about the type of contacts you want to filter or types of people you want to exclude. For example, search for contacts that are male, younger than 25, and live within 15 miles of Seattle, Washington.

To accomplish this, first click on Advanced Search. This presents specific fields that you can search through.

![Advanced Search](/articles/contacts/contacts-11.png "Advanced Search")

Using the options in Advanced Search you can narrow your list of contacts to only those that specifically match the criteria you are looking for.

![Advanced Search](/articles/contacts/contacts-12.png "Advanced Search")

After completing the form and clicking search, you can easily create a new segment froom your search results where the search parameters are automatically added to your segment to create a Dynamic Segment that will automatically be udpated for you.  

Advnaced users can also use the search paramters contained in the URL of the browser after their search to save, share or modify the URL directly.

`https://us-1.dailystory.com/Contact/?s=&gender=Male&location_q=Seattle,%20WA&distance=15&ageTo=25`

Contacts can have user defined attributes. Enterprise customers of DailyStory can configure those properties for search. When the user defined attribute is searchable it is available in advanced search.

For example, if your contact data is augmented with eligibility date and income data, and those fields are available to search, you will find the fields in advanced search.

![User Defined Search](/articles/contacts/contacts-13.png "User Defined Search")

> Indexing of custom Contact Properties, such as those shown above, are only available to Enterprise customers of DailyStory.

For more examples of search, [see advanced search examples](/contacts/advanced-search).

The Export button found at the bottom of All Contacts will be limited to the results defined in the search.

##Adding Contacts
Contacts are manually added through the + Add Contact button on the All Contacts page, Bulk Contact Import, or through the API.

Contacts are automatically added when someone completes a Web Form, Magic Form, or any other type of form associated with DailyStory if the contact does not already exist. A contact will also be created when a new lead is created and the underlying contact does not exist.

###Add a Contact
To add a single contact, click the + Add Contact button. This opens the Create a Contact form. The only field required to create a new contact is an email address.

###Bulk Contact Import
To bulk import contacts use the [bulk contact import](import) tool.

## Custom Contact Fields
Custom Contact Fields enable you to add custom fields to your contact.

### Add Custom Fields
To add custom fields for your contacts: 

1. Go to Contacts > All Contacts. 
2. Click the down arrow to the right of the + Add Contact button.
3. Select Custom Fields.

![Custom Fields](/articles/contacts/contacts-14.png "Custom Fields")

This opens the Manage Custom Fields screen. This screen enables you to add an unlimited number of custom fields for your contacts. 

These fields are available through the DailyStory API and are available for use in [personalization](/personalization). To use a custom field in a personalization script prefix the API with <code>Profile</code>. For example, to access a custom field such as Date Eligible: {{profile.date_eligible}}.

> DailyStory Professional and Enterprise customers can enable indexing of these custom fields for use in [segmentation](/segments).

4. Next, click the "Add" button. This opens a popup where you add the name of the field, select the type (Text, Number, Date/Time, Yes or No, True or False).

![Custom Fields](/articles/contacts/contacts-17.png "Custom Fields")

### Available Custom Field types
The table below lists the available custom field data types.

<table class="table">
<thead>
<tr>
<td style="width:25%"><strong>Field Type</strong></td>
<td><strong>Used For</strong></td>
</tr>
</thead>
<tbody>
<tr>
<td><code>Text</code></td>
<td>Used any text value or values that are not used in ranged searches. For example, a member id should be marked as `Text`, but number of purchases should be `Number`.</td>
</tr>
<tr>
<td><code>Number</code></td>
<td>Used for values that can be used in ranged searches. For example, number of purchases.</td>
</tr>
<tr>
<td><code>Date/Time</code></td>
<td>Date values, such as eligibility date.</td>
</tr>
<tr>
<td><code>Yes or No</code></td>
<td>Value must either by: `Yes` or `No`.</td>
</tr>
<tr>
<td><code>True or False</code></td>
<td>Value must either by: `True` or `False`.</td>
</tr>
</tbody>
</table>

Once added, your custom field is shown in the list of custom fields:

![Custom Fields](/articles/contacts/contacts-15.png "Custom Fields")

The custom field is now available: 

* As a mapping option when importing contacts; 
* As a mapped field in Web Forms and Magic Forms; 
* And as an editable field when editing a contact.

![User Defined Fields](/articles/contacts/contacts-16.png "User Defined Fields")
