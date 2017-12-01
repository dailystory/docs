{
title: 'Emails',
description: 'DailyStory Email'
}
# Emails
DailyStory Emails enable you to create personalized and targeted emails that can be sent to DailyStory [Contacts](/contacts) as part of a [Campaign's Workflow](/campaigns).

By using DailyStory's email marketing feature, DailyStory can track and attribute delivery, bounces, opens, and clicks to your DailyStory campaign.

DailyStory emails can be sent through the @dailystory.net mail server or you can add integration with a transactional email platform such as [Mailgun](/integrations/mailgun), SendGrid or PostMark.

> The benefit of using an integrated transactional email platform to send your email is you can configure your own sending email domain. If not, your email send address will appear as `sales@example.com on behalf of @dailystory.net`

## Creating and Editing Emails
Creating and editing emails within the DailyStory email editor is simple and intuitive.

On the top menu select Content > Emails:

![Emails Menu](/articles/emails/emails-01.png "Email Menu")

This will open up a page listing All Emails. From here you can select an existing email to edit or click the + New Email button to create a new email.

> This page also provide some insights into Delivered, Opened, Clicked and Bounced statistics for emails.

Clicking on any of the numbers for Delivered, Opened, Clicked and Bounced will open reports for the email.

![All Emails](/articles/emails/emails-02.png "All Emails")

Clicking + New Email will open up the New Email editor. When the page opens you will first need to select the [campaign](/campaigns) the email will be associated with.

> If you create an email in one campaign and want to use it in another campaign, just edit the email and click 'Create a Copy'

After selecting a campaign, you will be presented with the DailyStory email editor:

![New Email](/articles/emails/emails-03.png "All Email")

The email editor has 3 tabs and you can use any of them for authoring your email.

* **Live Edit** - provides a view similar to what your final email will look like.
* **Rich Edit** - provides a rich, WYSIWYG editor with helpful toolbars for common formatting options.
* **HTML (Advanced)** - edit the raw HTML used in your email.

> For sending HTML emails, be sure and include the  `<!DOCTYPE html>` and `<html> <head> <body>` tags.

On the right you will find a list of [merge tags](/reference#merge-tag) that you can use within your email. 

DailyStory makes extensive use of merge tags throughout the product and whenever possible we provide a list of the merge tags available.  

Finally, you can also select an [email template](/features/email-templates). An email template enables you to create a re-usable layout. If you select an email template, you only need to provide the content in the email body.

### Required Email Fields
DailyStory Emails require you provide a from address, a subject and a body.
#### To
The To: address will be set automatically when the email is used within a workflow or sent via the API. 

If a contact only has an email address, only the email address will be used. If the contact has a first or last name the email will be formatted as `First Last <email@example.com>`.
#### From
The From address must be a valid email address. For example:

* <code>Renew your membership &lt;sales@somecorp.com&gt;</code>
* <code>Rob Howard &lt;rob@dailystory.com&gt;</code>
* <code>hello@dailystory.com</code>

> A good best practice is to use a descriptive name in the from if the email isn't coming from a person.
#### Subject
The Subject should be a descriptive introduction to the body of your email message. The subject may contain merge tags.
#### Body
The Body of your email contains the message you want to send. The body may contain merge tags.

> While it is possible to edit the HTML of the email and use style sheets, be aware that it is best to use inline styles as most email clients do not recognize style sheets.

### Email Merge Tags
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

Any merge tags used in the email that doesn't exist for the contact you are sending to is automatically removed.

For example if the <code>\*|FNAME|\*</code> merge tag was used, but the contact does not have a Firstname field this:	 <code>Hi \*|FNAME|\*</code> Becomes: <code>Hi</code>

## Testing your Email
There are several options for testing emails.

### Send a test email
Use the Sent a test email button to send yourself (or someone else) a test email.

> Important, you must save your email prior to sending a test email. And, the test emails you send count towards your monthly send limits.

![Send test email](/articles/emails/emails-04.png "Send test email")

Clicking Send a test email will open up a window. Enter a valid email address to send your test email to.

![Test email recipient]/articles/emails/emails-05.png "Test email recipient")

The test email will use the [Test Contact](/reference#test-lead) for any merge fields found in the email.

### Email Addresses DailyStory Ignores
For testing and demonstration purposes you can use recipient addresses ending in <code>@test.com</code> and <code>@example.com</code>. These email addresses do not count towards your license limits and these emails will never be sent.

If you want to test sending emails, such as running a test lead through a workflow, we recommend using a disposable email address such as <a href="http://www.fakemailgenerator.com/" rel="noopener noreferrer">Fake Mail Generator</a>.

## Email Reporting
You can review a summary of your email delivery by clicking on the Delivered number from the All Emails page. This will open the Email Delivery Report:

![Email Delivery Report](/articles/emails/emails-06.png "Email Delivery Report")

You can also click on Opened, Clicked, and Bounced for each email in the All Emails page. To view who opened the email, clicked on a link in the email or bounced. These reports are also accessible as links in the Email Delivery Report.

The Email Delivery Report provides visuals for sent/deliver/bounced and related percentages for each. The sent/delivered/bounced graph is shown in the image above.

Next, you will find a graph detailing delivered/opened emails. You can also click on the link in the graph to see who opened the email.

![Email Delivery Report Opens](/articles/emails/emails-08.png "Email Delivery Report Opens")

After the delivered/opened graph you will find the opened/clicked report. You can also click on the link in the graph to see who clicked the email.

![Email Delivery Report Clicks](/articles/emails/emails-09.png "Email Delivery Report Clicks")

### Bounced Email Report
The Bounced Email Report provides a list of contacts that whose email address bounced for the sent email. The report can be filtered by time ranges and exported to a file that can be opened in Excel.

![Email Bounce Report](/articles/emails/emails-10.png "Email Bounce Report")

> Export files are scoped to the date range your select when viewing your report.

### Opened Email Report
The Opened Email Report provides a list of which contacts opened the email. The report can be filtered by time ranges and exported to a file that can be opened in Excel.

![Email Opened Report](/articles/emails/emails-07.png "Email Opened Report")

> Export files are scoped to the date range your select when viewing your report.

### Clicked Email Report
The Clicked Email Report provides a list of which contacts clicked a link in the email. The report can be filtered by time ranges and exported to a file that can be opened in Excel.

![Email Clicked Report](/articles/emails/emails-11.png "Email Clicked Report")

> Export files are scoped to the date range your select when viewing your report.