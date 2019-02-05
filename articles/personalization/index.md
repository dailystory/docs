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

## Personalization fields
Below is a list of DailyStory's built-in fields available for personalization:


### Contact field properties
The following personalization properties are unique to each individual contact.

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


### Organization field properties
The following personalization properties are global to your account within DailyStory.

* `{{organization.name}}`
* `{{organization.industry}}`
* `{{organization.url_website}}`
* `{{organization.url_appstore_google}}`
* `{{organization.url_appstore_ios}}`
* `{{organization.url_facebook}}`
* `{{organization.url_instagram}}`
* `{{organization.url_linkedin}}`
* `{{organization.url_pintrest}}`
* `{{organization.url_twitter}}`
* `{{organization.url_youtube}}`

### Custom profile field properties
Custom profile field properties are [properties you add to your profile](https://docs.dailystory.com/contacts/#user-defined-fields).

When you add a custom profile field you will see a corresponding API Name associated with your profile field:

![User Defined Fields](/articles/contacts/contacts-15.png "User Defined Fields")

To use a custom profile field in DailyStory's Personalization Engine prefix the API name with `profile`.

For example, to reference the Has Donated custom field: `{{profile.has_donated}}` 


## Features available for personalization
The Personalization Engine is available for the following features:

