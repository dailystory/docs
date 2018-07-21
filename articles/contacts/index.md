{
title: 'Contacts',
description: 'A DailyStory Contact is a customer or prospective customer managed by DailyStory.'
}
#Contacts
A DailyStory Contact is a customer or prospective customer managed by DailyStory. 

While there is only a single contact for an individual managed by DailyStory, the contact may be part of multiple campaigns. For example, a contact can be subscribed to a newsletter, part of a nuturing drip campaign, and part of a new membership email sequence.

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

After completing the form and clicking search, the URL of the browser contains the search parameters. This is useful because you can save the URL, share the URL, and more advanced users modify the URL directly.

`https://us-1.dailystory.com/Contact/?s=&gender=Male&location_q=Seattle,%20WA&distance=15&ageTo=25`

Contacts can have user defined attributes. Enterprise customers of DailyStory can configure those properties for search. When the user defined attribute is searchable it is available in advanced search.

For example, if your contact data is augmented with elibibility date and income data, and those fields are available to search, you will find the fields in advanced search.

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

##User Defined Fields
To add user defined fields for your contacts go to Contacts > All Contacts. Next, click the down arrow to the right of the + Add Contact button and select Contact Fields.

![User Defined Fields](/articles/contacts/contacts-14.png "User Defined Fields")

This opens the Manage Contact Profile Fields which enables you to add an unlimited number of custom fields for your contacts. These fields are available through the DailyStory API and are available for use in personalization.

> DailyStory Enterprise customers can additionally enable search indexing of these user defined contact fields.

Simply add the name of the field you want to add, select the type (Text, Number, Date/Time, Yes or No, True or False) and then add your field.

![User Defined Fields](/articles/contacts/contacts-15.png "User Defined Fields")

Your user defined field is now available as a mapping option when importing contacts, as a mapped field in Web Forms and Magic Forms, and as an editable field when editing a contact.

![User Defined Fields](/articles/contacts/contacts-16.png "User Defined Fields")