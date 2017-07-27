---
layout: _ArticleLayout
title: Emails
description: Emails managed by DailyStory
---
#DailyStory Emails
DailyStory Emails enable you to create personalized and targeted emails that can be sent from any person or alias, such as 'support', within your organization. This is different than bulk marketing emails such as a newsletter.

> In fact while DailyStory can be used to send bulk emails, we don't recommend it.

Additionally, DailyStory supports integration with several transactional email systems. Our transactional email platform of choice is [Mailgun](https://www.mailgun.com). 

> Unless you select an alternative all of your emails will be sent through our [Mailgun integration](/integrations/mailgun) with a sending domain of dailystory.net.

## Creating and Editing Emails
Creating and editing emails with the DailyStory email editor is simple and intuitive.

On the top menu select Content > Emails:

![Emails Menu](/articles/features/emails-01.png "Email Menu")

This will open up a page listing All Emails. From here you can select an existing email to edit or click the + New Email button to create a new email.

> This page also provide some insights into Delivered, Opened, Clicked and Bounced statistics for emails.

![All Emails](/articles/features/emails-02.png "All Emails")

### Create Email
Clicking + New Email will open up the New Email page. When the page opens you will first need to select the [campaign](/campaigns) the email will be associated with.

> If you create an email in one campaign and want to use it in another campaign, just edit the email and click 'Create a Copy'

After selecting a campaign, you will be presented with the DailyStory email editor:

![New Email](/articles/features/emails-03.png "All Email")

The email editor has 3 tabs and you can use any of them for authoring your email.

* **Live Edit** - provides a view similar to what your final email will look like.
* **Rich Edit** - provides a rich, WYSIWYG editor with toolbars.
* **HTML (Advanced)** - edit the raw HTML used in your email.

On the right you will find a list of [merge tags](/reference#merge-tag) that you can use within your email. 

> DailyStory makes extensive use of merge tags throughout the product and whenever possible we provide a list of the merge tags available.  

Finally, you can also select an [email template](/features/email-templates). An email template enable you to create a reusable layout and then add your email's body content to that layout.

#### Required Email Fields
Emails require that you provide a from address, a subject and a body.

> The To: address will be set automatically when the email is used within a workflow or sent via the API.

The From address must be a valid email address. For example:

* <code>Renew your membership &lt;sales@somecorp.com&gt;</code>
* <code>Rob Howard &lt;rob@dailystory.com&gt;</code>
* <code>hello@dailystory.com</code>

> A good best practice is to use a descriptive name in the from if the email isn't coming from a person.

The Subject should be a descriptive introduction to the body of your email message.

The Body of your email contains the message you want to send.

> While it is possible to edit the HTML of the email and use style sheets, be aware that it is best to use inline styles as most email clients do not recognize style sheets.

#### Email Merge Tags
In both the subject and body of your email you can include Merge Tags:
<table class="table">
<tbody>
<tr>
<td><strong>Merge Tag</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code>*|FNAME|*</code></td>
<td>The recipient's first name</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|LNAME|*</code></td>
<td>The recipient's last name</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|FULLNAME|*</code></td>
<td>The recipient's full name</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|COMPANY|*</code></td>
<td>The recipient's company name</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|EMAIL|*</code></td>
<td>The recipient's email address</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|DATE|*</code></td>
<td>The current date</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|TIME|*</code></td>
<td>The current time</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|TITLE|*</code></td>
<td>The recipient's title</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|LOGO|*</code></td>
<td>The logo configured for your tenant</td>
</tr>
<tr>
<td width="25%" nowrap><code>*|UNSUBSCRIBE|*</code></td>
<td>An unsubscribe url</td>
</tr>
</tbody>
</table>

> Important, if an <code>\*|UNSUBSCRIBE|\*</code> merge tag is not found an unsubscribe link will automatically be included in the email. An unsubscribe header with this link is also sent as part of the email - these are best practices to ensure the email is not flagged as SPAM.

Any merge tags used in the email that don't exist for the contact you are sending to are automatically removed.

For example if the <code>\*|FNAME|\*</code> merge tag was used, but the contact does not have a Firstname field this:	 <code>Hi \*|FNAME|\*</code> Becomes: <code>Hi</code>

### Edit Email
	

