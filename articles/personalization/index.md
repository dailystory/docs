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

* `{{user.fullname}}` - string; full name of the contact.
* `{{user.firstname}}` - string; first name of the contact.
* `{{user.lastname}}` - string; last name of the contact.
* `{{user.email}}` - string; email address of the contact.
* `{{user.country}}` - string; country of the contact.
* `{{user.region}}` - string; region or state of the contact.
* `{{user.city}}` - string; city of the contact.
* `{{user.address}}` - string; address of the contact.
* `{{user.postalcode}}` - string; postal or zip code of the contact.
* `{{user.title}}` - string; title of the contact.
* `{{user.phone}}` - string; phone number of the contact.
* `{{user.mobile}}` - string; mobile phone number of the contact.
* `{{user.website}}` - string; url of the contact.
* `{{user.gender}}` - string; gender of the contact.
* `{{user.age}}` - number; age of the contact.
* `{{user.lastModified}}` - date; when the contact was last modified.
* `{{user.lastContacted}}` - date; when the contact was last contacted.

### Organization field tokens
The following personalization tokens are related to the organization the contact belongs to.

* `{{organization.name}}` - string; name of the company or organization the contact is part of.
* `{{organization.industry}}` - number; industry code number the contact is part of.

### Account field tokens
The following personalization tokens are global to your account within DailyStory.

* `{{account.name}}` - string; name of the account.
* `{{account.url_website}}` - string; url to the account's website.
* `{{account.url_appstore_google}}` - string; url to the account's Android App download.
* `{{account.url_appstore_ios}}` - string; url to the account's Apple App download.
* `{{account.url_facebook}}` - string; url to the account's Facebook page.
* `{{account.url_instagram}}` - string; url to the account's Instagram page.
* `{{account.url_linkedin}}` - string; url to the account's LinkedIn page.
* `{{account.url_pintrest}}` - string; url to the account's Pintrest page.
* `{{account.url_twitter}}` - string; url to the account's Twitter page.
* `{{account.url_youtube}}` - string; url to the account's YouTube page.

### System tokens
The following tokens are tokens that evaluate to common values and are useful for comparisons.

* `{{system.today}}` - date; evaluates to today's date localized for your account.

> Many of the account tokens are built into templates and designers. For example, the URLs set for App download or Social buttons in the email designer are automatically set using the Account personalization tokens.

### Custom profile tokens
Custom profile tokens correspond to [custom fields you can add to your contact](https://docs.dailystory.com/contacts/#user-defined-fields).

When you add a custom profile field you will see a corresponding API Name:

![User Defined Fields](/articles/contacts/contacts-15.png "User Defined Fields")

> To use a custom profile token in DailyStory's Personalization Engine prefix the API name with `profile`.

For example, to reference the Has Donated custom field shown above use the token: `{{profile.has_donated}}` 

## Using conditions
The DailyStory Personalization Engine automatically replaces the personalization token with the content associated with it. 

For example, for a contact whose first name is 'Anna' the personalization token `{{user.firstname}}` is replaced with `Anna`. 

But what happens when the token is not set? Such as when you write an email and start with a salutation, such as:

`Hi {{user.firstname}},`

If the contact's first name is not set, this becomes:

`Hi ,`

Instead, this should be replaced with a conditional statement: if the contact has a first name, use it. If they don't have a first name, replace it:

`{{#if user.firstname}}Hi {{user.firstname}},{{else}}Hi,{{/if}}`

Now, when the first name is blank, this is what the Personalization Engine outputs:

`Hi,`

### If / else
The most basic conditional statement is `{{#if}}`. This simply checks if a profile field exists.

This can be as simple as:

`{{#if account.url_facebook}}Visit our page on Facebook{{/if}}`

Or, using the `{{else}}` statement, show an alternative if the field was empty:

`{{#if user.firstname}}Hi {{user.firstname}},{{else}}Hi,{{/if}}`

> Note, you can use personalization tokens within the output of conditional statements.

### If equals / else
The basic if / else condition checks if a value is empty. The if equals check evaluates whether the token matches a specific value. For example, checking if a contact's country is 'Canada':

<code>
{{#ifEqual profile.country 'Canada'}}
Hey there Canada!
{{/ifEqual}}
</code>

> String evaluations are not case sensitive. In the above example, 'canada', 'Canada' or 'CANADA' would all evaluate as equal.

An else condition is also supported for `{{#ifEqual}}`:

<code>
{{#ifEqual profile.country 'Canada'}}
Hey there Canada!
{{else}}
You aren't Candadian!
{{/ifEqual}}
</code>

### If condition / else
The basic if / else condition checks if a value is empty. While useful, sometimes you need more complex evaluations. For example, checking if a contact's membership is about to expire:

<code>
{{#ifCond profile.membership_expiration_date '>' '2019-06-01'}}
Your membership has expired.
{{/ifCond}}
</code>

The `{{#ifCond}}` evaluates a personalization token against a value using:

* `=` - equals
* `<` - less than
* `>` - greater than
* `<>` or `!=` - not equal
* `<=` - less than or equal to
* `>=` - greater than or equal to

> Important the evaluators <= and >= are only valid when evaluating numbers and dates.

An else condition is also supported for `{{#ifCond}}`:

`{{#ifCond profile.membership_expiration_date '>' '2019-06-01'}}`
`Your membership has expired.`
`{{else}}`
`Your membership is in good standing.`
`{{/ifCond}}`

### Multiple conditions
In the examples referenced above, all of the conditions are if/else. This limits your personalization because it requires to you match a condition. But what about when you can match for muliple conditions? While slightly more complex, the `{{#switch}}` statement supports multiple matching options:

`{{#switch user.country}}`
`{{#case 'Canada'}}Hello Canada!{{/case}}`
`{{#case 'United States'}}Hello United States!{{/case}}`
`{{/switch}}`

> The `{{#switch}}` personaliation condition is currently only available for string evaluations.

## Features available for personalization
The Personalization Engine is available for the following features.

### Email
The use of Personalization within [email](/emails) is available in:

* Subject
* Preview Text 
* Body
* Plain text Body

### Text Messages
The use of Personalization within [text messages](/text-messages) is available in:

* Message body

### Push Notifications
The use of Personalization within [push notifications](/push-notifications) is available in:

* Title
* Message body

## Related articles

* [Personalization is one-to-one marketing](https://www.dailystory.com/blog/personalization-email-targeting/)
* [Personalized email marketing for everyone](https://www.dailystory.com/features/personalized-email-marketing/)