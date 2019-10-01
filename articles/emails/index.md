
{
title: 'Email Marketing',
description: 'DailyStory email marketing'
}
# DailyStory Email Marketing
Email Marketing sends targeted and personalized email to your [Segments](/segments) and [Contacts](/contacts) in a [Campaign](/campaigns). Emails are either sent based on a [Schedule](/campaigns/schedules) or a [Workflow](/campaigns/workflows).

DailyStory tracks and attributes delivery, bounces, opens, clicks, and optouts automatically.

Unless otherwise specified, email is sent by DailyStory from an @dailystory.net email address. However, it is strongly recommend that you configure a custom domain to allow DailyStory to send email securely on your behalf or leverage DailyStory's [Mailgun](/integrations/mailgun), SendGrid or PostMark integrations.

> Enabling DailyStory to send email from your domain name increases the likelihood that your email is successfully delivered. Otherwise, your email send address will appear as `sales@[your domain].com on behalf of @dailystory.net`

This guide provides a list of resources to help you get started with DailyStory email.

**Create and Edit an Email**

* [Create an Email](#create-an-email)
* [Edit an Email's Settings](#edit-an-email)
* [Email Designer](#email-designer)

**Advanced Tracking Link Options**

* [Tracking Ad Clicks](#tracking-ad-clicks)
* [Integrate with Google Analytics](#integrate-with-google-analytics)
* [Advanced Options](#advanced-options)

**Reporting and Metrics**

* [Conversion Tracking](#conversion-tracking)
* [Click Tracking](#click-tracking)

**Frequently Asked Questions**


FAQ
What happens if an email bounces
What is a soft bounce?
Will DailyStory try and resend soft bounces?

## Create an Email <a name="create-an-email"></a>
To create an email, first navigate to Content > Emails. This will display All Emails. From here you can create a new blank email or a new email from a template: ![Menu Button](https://docs.dailystory.com/articles/emails/emails-01.png "All Email") 

You can all also click the menu in the top left and click "+ Create" to create a new blank email:

![Emails Menu](https://docs.dailystory.com/articles/emails/emails-14.gif "Email Menu")

Next, you will be taken to the Email Settings screen. When the page opens you will first need to select the [campaign](/campaigns) the email will be associated with.

> Later, if you want to use this email in another campaign, click 'Create a Copy'. 

After selecting a campaign, you are presented with the Create Email screen:

![Create Email](https://docs.dailystory.com/articles/emails/emails-03.png "Create Email")

On the Create Email screen there are a number of fields:

 - **Name** - The name of your email within DailyStory.
 - **Description** - The description of your email within DailyStory.
 - **Subject** - The subject of your email.
 - **From** - The from address of your email.
 - **Preview** - The preview text of your email.

The **Subject** of your email is a descriptive introduction to the body of your email message. The subject may contain emojis and personalization tags or script.

The **From** address must be a valid email address. Examples:

* <code>Renew your membership &lt;sales@somecorp.com&gt;</code>
* <code>"Rob Howard" &lt;rob@dailystory.com&gt;</code>
* <code>hello@dailystory.com</code>

Clicking the more options dots to the right of the **From** address will open a popup. From this popup edit the friendly name, email and where replies should be sent to:

![Set from address](https://docs.dailystory.com/articles/emails/emails-15.gif "Set from address")

> You can also type or paste in the email address too.

Use **Preview** to optionally write content shown when the email is previewed in your recipient's inbox. This enables you to control exactly what is seen when someone is previewing your email in their inbox. The preview may contain emojis and personalization tags or script.

Once the required fields (Name, Subject and From) are complete, click the "Create Email" to create the new email.

Next, you can either <a href="#edit-html">edit the HTML</a> of the email or use the <a href="#email-designer">Email Designer</a> to build a new email.

## Edit an Email's Settings<a name="edit-an-email"></a>
When an email is selected from the All Emails list, the default action is to navigate to the Email Designer. 

To edit settings, such as the From address and Subject of the email click on the more options button to the right of an email. This will open a list of actions available for this email.

![Edit email settings](https://docs.dailystory.com/articles/emails/emails-16.gif "Edit email settings")

## Email Designer<a name="email-designer"></a>
Clicking on an email from the All Emails list or clicking the Design Email button from the Email Settings will open the Email Designer.

> While it is possible to edit the HTML of the email, we recommend only editing the HTML when creating a new email template. 

![Email Designer](https://docs.dailystory.com/articles/emails/emails-17.png "Email Designer")

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

Merge tags provide a simple way to personalize your email, but do have limitations. For more robust personalization of your [email use personalization templates](https://www.dailystory.com/features/personalized-email-marketing/#templating-in-your-personalized-email-marketing).

### Email Personalization Templates
Personalization templates provide all the same functionality as merge tags for personalization. 

> Personalization Templates don't exist for merge tags such as <code>\*|BODY|\*</code>, <code>\*|WEBVIEW|\*</code>, <code>\*|UNSUBSCRIBE|\*</code>.

Personalization templates use a separate format. For example, to insert the user's first name use <code>{{user.firstname}}</code>

[UNDONE]

## Advanced Options
DailyStory includes advanced options for emails such as setting an email preheader and including a web view of the email.

### Setting an Email Preheader
The majority of email clients provide a snippet of text to preview the contents of an email in your inbox. This enables you to quickly scan your inbox and decide if you want read, save, or archive the email.

This inbox preview text can be set using an [email preheader](https://www.dailystory.com/blog/email-preheader-improve-open-rates/).

To set an email preheader click the Advanced Options tab. There you'll find an option to set the preheader.

![PreHeader Text](/articles/emails/emails-12.png "PreHeader Text")

This will include a hidden HTML div in the body of your email:
	
<pre class="brush: html">
&lt;div class="preheader" style="display:none !important;
visibility:hidden !important;
mso-hide:all !important;
font-size:1px;
overflow:hidden !important;
display:none !important;"&gt;
The contents of your preheader text
&lt;/div&gt;
</pre>

### Enabling Email Web View
A web view of your email enables people to click a link in your email and view the email in a web browser.

> By default web view is disabled and no web view is available for your email.

To enable a web view of your email first enable the web view by clicked the toggle button on the Advanced Options tab:
	
![Enable Web View](/articles/emails/emails-13.png "Enable Web View")

Next, use the <code>\*|WEBVIEW|\*</code> merge tag to include a link in your email.

> Note, the <code>\*|WEBVIEW|\*</code> merge tag only inserts the URL.

Optionally use the preview link next to the web view toggle button to preview what the web view of your email looks like. It will be personalized using the [Test Contact](/reference#test-lead).

The web view of the email is unique to each recipient. If personalization or merge tags are used in the email people who view the link will see the personalized view.

## Testing your Email
There are several options for testing emails. You can create a test campaign, add your email as a workflow and then add leads to the campaign. However, to test only the email, just use the Send a test email button in the email editor.

### Send a test email
Use the Sent a test email button to send yourself (or someone else) a test email.

> Important, you must save your email prior to sending a test email. Test emails count towards your monthly send limits.

![Send test email](/articles/emails/emails-04.png "Send test email")

Clicking Send a test email will open up a window. Enter a valid email address to send your test email to.

![Test email recipient](/articles/emails/emails-05.png "Test email recipient")

The test email will use the [Test Contact](/reference#test-lead) for any merge fields found in the email.

### Email Addresses DailyStory Ignores
For testing and demonstration purposes you can use recipient addresses ending in <code>@test.com</code> and <code>@example.com</code>. These email addresses do not count towards your license limits and these emails will never be sent.

If you want to test sending emails, such as running a test lead through a workflow, we recommend using a disposable email address such as <a href="http://www.fakemailgenerator.com/" rel="noopener noreferrer">Fake Mail Generator</a>.

## Email Reporting
Emails sent through DailyStory include detailed delivery reporting. You can review a summary of your email delivery by clicking on the Delivered number from the All Emails page. This will open the Email Delivery Report:

![Email Delivery Report](/articles/emails/emails-06.png "Email Delivery Report")

> You can also click on Opened, Clicked, and Bounced for each email in the All Emails page to view who opened the email, clicked on a link in the email or bounced. These reports are also accessible as links in the Email Delivery Report.

The report provides several graphs to help you visualize your email delivery performance. 

The first graph, shown in the image above, details sent/deliver/bounced along with % delivered for the selected date range.

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