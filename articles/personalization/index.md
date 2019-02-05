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
Below is a list of DailyStory's built in fields available for personalization:

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


## Features available for personalization
The Personalization Engine is available for the follwing features:

