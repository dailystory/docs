{
title: 'DailyStory Personalization',
description: 'Personalize and target content based on individual contact properties.'
}
#DailyStory Personalization
Use DailyStory's Personalization Engine to create content individually targeted to a contact's profile properties.

Personalization is as simple as displaying a person's firstname, `{{user.firstname}}`, or as complex as showing different content if the person's firstname profile was not set:

`{{#if user.firstname}}Hi {{user.firstname}},{{else}}Hi,{{/if}}`

Personalization is available for both built-in properties, such as firstname, as well as any custom property you add.

> DailyStory's Personalization Engine uses opening and closing braces `{{` and `}}` to signify markup the Personalization Engine needs to process.

## Personalization tokens
Below is a list of DailyStory's built-in tokens available for personalization:

### Contact field tokens
The following personalization tokens are unique to each individual contact.

* `{{user.fullname}}`
* `{{user.firstnam}}`
* `{{user.lastname}}`
* `{{user.email}}`
* `{{user.country}}`
* `{{user.region}}`
* `{{user.city}}`
* `{{user.address}}`
* `{{user.postalcode}}`
* `{{user.title}}`
* `{{user.phone}}`
* `{{user.mobile}}`
* `{{user.website}}`
* `{{user.gender}}`
* `{{user.age}}`
* `{{user.lastModified}}`
* `{{user.lastContacted}}`

### Organization field tokens
The following personalization tokens are related to the organization the contact belongs to.

* `{{organization.name}}`
* `{{organization.industry}}`

### Account field tokens
The following personalization tokens are global to your account within DailyStory.

* `{{account.name}}`
* `{{account.url_website}}`
* `{{account.url_appstore_google}}`
* `{{account.url_appstore_ios}}`
* `{{account.url_facebook}}`
* `{{account.url_instagram}}`
* `{{account.url_linkedin}}`
* `{{account.url_pintrest}}`
* `{{account.url_twitter}}`
* `{{account.url_youtube}}`

> Many of the account tokens are built into templates and designers. For example, the URLs set for App download or Social buttons in the email designer are automatically set using the Account personalization tokens.

### Custom profile tokens
Custom profile tokens correspond to [custom fields you can add to your contact](https://docs.dailystory.com/contacts/#user-defined-fields).

When you add a custom profile field you will see a corresponding API Name:

![User Defined Fields](/articles/contacts/contacts-15.png "User Defined Fields")

> To use a custom profile token in DailyStory's Personalization Engine prefix the API name with `profile`.

For example, to reference the Has Donated custom field shown above use the token: `{{profile.has_donated}}` 

## Using conditions
The DailyStory Personalization Engine automatically replaces the personalization tokens. For example, for a contact whose first name is 'Anna' the personalization token `{{user.firstname}}` is replaced with `Anna`. 

But what happens when the token is not set? Such as when you write an email and start with a salutation, such as:

`Hi {{user.firstname}},`

If the contact's first name is not set, this becomes:

`Hi ,`

Instead, this should be replaced with a conditional statement: if the contact has a firstname, use it. If they don't have a first name, replace it:

`{{#if user.firstname}}Hi {{user.firstname}},{{else}}Hi,{{/if}}`

Now, when the firstname is blank, this is what the Personalization Engine outputs:

`Hi,`

### If / else conditions
The most basic conditional statement is `{{#if}}`. This simply checks if a profile field exists.

This can be as simple as:

`{{#if account.url_facebook}}Visit our page on <a href="{{account.url_facebook}}">Facebook</a>{{/if}}`

Or, using the `{{else}}` statement, show an alternative if the field was empty:

`{{#if user.firstname}}Hi {{user.firstname}},{{else}}Hi,{{/if}}`



## Features available for personalization
The Personalization Engine is available for the following features:

