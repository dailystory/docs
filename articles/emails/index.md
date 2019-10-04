{
title: 'DailyStory Email Marketing',
description: 'DailyStory email marketing'
}
# DailyStory Email Marketing
DailyStory/s Email Marketing engine sends targeted and personalized email to your [Segments](/segments) and [Contacts](/contacts) in a [Campaign](/campaigns). Emails are sent based on a [Schedule](/campaigns/schedules) or a [Workflow](/campaigns/workflows). You can also send individual emails.

DailyStory tracks and attributes delivery, bounces, opens, clicks, and optouts automatically.

Unless otherwise configured, email is sent by DailyStory from an @dailystory.net email address. However, it is strongly recommend that you configure a custom domain to allow DailyStory to send email securely on your behalf or leverage DailyStory's [Mailgun](/integrations/mailgun), SendGrid or PostMark integrations.

> Enabling DailyStory to send email securely from your domain increases the likelihood that your email is successfully delivered. Otherwise, your sending email address will appear as `[your name]@[your domain].com on behalf of @dailystory.net`

This guide provides a list of resources to help you get started with DailyStory email.

**Create and Edit an Email**

* [Create an Email](#create-an-email)
* [Edit an Email's Settings](#edit-an-email)
* [Email Designer](#email-designer)
* [HTML Editor](#edit-html)
* [Preview Email](#preview)
* [Send Test](#test)

[**Sending an Email**](#send)

* [Schedule Email to Send](#schedule)
* [Send a Single Email](#single)
* [Sending Rules and Guardrails](#send-rules)
* [Personalization](https://docs.dailystory.com/personalization)
* [Merge Tags](#merge-tags)

**Advanced Email Options**

* [Edit CSS](#edit-css)
* [Edit Plain Text](#edit-plaintext)
* [Import or Export an Email](#export)

[**Reporting and Metrics**](https://docs.dailystory.com/emails/reports)

[**Frequently Asked Questions**](#faq)

* [Why do emails look different across email clients?](#email-clients)
* [What email addresses are ignored?](#ignored-email-addresses)
* [What is an email preheader?](#faq-preheader)
* [Does DailyStory support Merge Tags?](#faq-merge-tags)
* [What happens if an email bounces?](#faq-bounce)
* [What is a soft bounce?](#faq-soft-bounce)
* [Will DailyStory try and resend soft bounces?](#faq-resend)

## Create an Email <a name="create-an-email"></a>
To create an email, first navigate to Content > Emails. This will display All Emails. From here you can create a new blank email or a new email from a template: 

![Menu Button](https://docs.dailystory.com/articles/emails/emails-01.png "All Email") 

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

The **Subject** of your email is a descriptive introduction to the body of your email message. The subject may contain emojis and [personalization tags and scripts](https://docs.dailystory.com/personalization).

The **From** address must be a valid email address. Examples:

* <code>Renew your membership &lt;sales@somecorp.com&gt;</code>
* <code>"Rob Howard" &lt;rob@dailystory.com&gt;</code>
* <code>hello@dailystory.com</code>

Clicking the more options dots to the right of the **From** address will open a popup. From this popup edit the friendly name, email address and where replies should be sent to:

> Set a "Send replies to" email address if you want replies to be sent to someone other than who the email came from.

![Set from address](https://docs.dailystory.com/articles/emails/emails-15.gif "Set from address")

> You can also type or copy/paste in the email **From** address too.

Use **Preview** to optionally write content shown when the email is previewed in your recipient's inbox. This enables you to control exactly what is seen when someone is previewing your email in their inbox. The preview may contain emojis and [personalization tags and scripts](https://docs.dailystory.com/personalization).

Once the required fields (Name, Subject and From) are complete, click the "Create Email" button to save the new email.

Next, you can either <a href="#edit-html">edit the HTML</a> of the email or use the <a href="#email-designer">Email Designer</a> to build a new email.

## Edit an Email's Settings<a name="edit-an-email"></a>
When an email is selected from the All Emails list, the default action is to navigate to the Email Designer. 

To edit settings, such as the From address and Subject of the email click on the more options button to the right of an email. This will open a list of actions available for this email.

![Edit email settings](https://docs.dailystory.com/articles/emails/emails-16.gif "Edit email settings")

## Email Designer<a name="email-designer"></a>
Clicking on an email from the All Emails list or clicking the Design Email button from Email Settings will open the Email Designer.

> While it is possible to edit the HTML of the email, we recommend only editing the HTML when creating a new email template. 

![Email Designer](https://docs.dailystory.com/articles/emails/emails-17.png "Email Designer")

The Email Designer is a drag-and-drop design canvas. To add an item to the designer canvas select a widget, such as a Text Section, by clicking and holding the mouse down and drag-and-drop it onto the design surface.

You will see a green bar that indicates where the designer will place your widget.

![Email Designer drag-and-drop](https://docs.dailystory.com/articles/emails/emails-18.gif "Email Designer drag-and-drop")

When the widget is added to the designer you can move, delete or edit the widget. Some of the design widgets have special options which will show up in place of the widgets.

The Email Designer generates HTML friendly emails optimized for common email clients such as Outlook, GMail and more. Furthermore, emails built within the designer are also optimized for mobile devices.

[Read more about the Email Designer in our Using the Email Designer guide](/emails/designer)

## HTML and CSS Editor<a name="edit-html"></a>
While DailyStory's Email Designer enables you to quickly build robust emails, more complicated email designs typically start from an HTML base.

As an example, if you have an existing email design you wish to use in DailyStory the best way to start is to copy-and-paste the HTML of that email as HTML and CSS.

![Email HTML Editor](https://docs.dailystory.com/articles/emails/emails-19.png "Email HTML Editor")

Editing the HTML of an email is an advanced option. And, emails built with the Email Designer will initially prevent you from editing the email:

![Email HTML Locked](https://docs.dailystory.com/articles/emails/emails-20.png "Email HTML Locked")

However, you can always click "Unlock HTML Editor" to edit the HTML.

> Editing the HTML of an email built with the designer may cause the designer to no longer recognize widgets added with the designer.

### Editing CSS<a name="edit-css"></a>
While editing the HTML of an email built with the designer is not recommended, the CSS of an email may be editing with no impact to the designer.

Simply click the CSS tab and edit/modify CSS rules for your email.

**Important** when DailyStory sends your email it merges all the CSS and HTML together. The full CSS is always included in a &lt;style&gt; tag of the HTML body of your email, but DailyStory will also attempt to inline the CSS rules as well. You can preview and email and view the source to see what the fully merged HTML of the email will look like.

### Editing the Plain Text<a name="edit-plaintext"></a>
Emails sent by DailyStory always include both an HTML version and a Plain Text version.

The plain text of the email is edited from the HTML Editor's "Edit Plain Text" tab. If not provided, DailyStory will attempt to automatically generate a plain text version of your content when the email is sent.

To learn more about using plain text in your email, see our article:
[Plain text or HTML email – which to use in your next campaign](https://www.dailystory.com/blog/plain-text-email/)

## Email Options Menu<a name="options"></a>
In both the Email Designer and HTML Editor, there is an options button in the top right:

![Options menu](https://docs.dailystory.com/articles/emails/emails-21.gif "Options menu")

Opening the options menu provides some additional features: [Preview](#preview), [Send Test](#test), [Schedule an Email](#schedule), quick navigation to the Email Designer or HTML Editor, Email Settings, and [Export](#export).

## Preview an Email<a name="preview"></a>
Prior to [sending an email](#send) we recommend previewing and [testing your email](#test).

To Preview an email, click the [options menu](#options) and click the Preview option. This will open a new tab and display a preivew of your email.

> Due to HTML inconsistencies sometimes the Preview will look slightly different than how the email appears in the Designer. The Preview is a more accurate view of how the final email will appear. You may need to make adjustments in the designer.

Use Preview to test your links, buttons, images and optionally view how the email will appear on mobile devices.

**Important** Any [Personalization](https://docs.dailystory.com/personalization) or [Merge Tages](#merge-tags) will use DailyStory's [test user data](https://docs.dailystory.com/reference#test-lead).

![Preview DailyStory email](https://docs.dailystory.com/articles/emails/emails-22.png "Preview DailyStory email")

## Send Test Email<a name="test"></a>
Prior to [sending an email](#send) we recommend [previewing](#preview) and testing your email.

To send a test email, click the [options menu](#options) and click the Send Test option. This will open a popup window pre-populated with your email.

**Important** Any [Personalization](https://docs.dailystory.com/personalization) or [Merge Tages](#merge-tags) will use DailyStory's [test user data](https://docs.dailystory.com/reference#test-lead).

The email is delivered to your inbox shortly thereafter.

![Send test](https://docs.dailystory.com/articles/emails/emails-23.png "Send test email")

Emails sent to your recipients [may look slightly different between email clients](#email-clients).

If you need to send an email to a contact, not for the purpose of testing the email. You can [send a single email](#single)

## Sending an Email<a name="send"></a>
After [previewing](#preview) and [testing](#test) your email, you are ready to schedule an email to send.

There are 3 ways you can send emails to your contacts:

* [Schedule an email](#schedule)
* [Send a single email](#single)
* [Send as part of a workflow](#workflow)

### Schedule an Email<a name="schedule"></a>
Scheduling an email is the easiest way to send an email to your contacts. From either the [Email Designer's](#email-designer) options or the [Email Settings](#edit-an-email) click Schedule to open the message scheduler:

![Schedule an email](https://docs.dailystory.com/articles/emails/emails-24.png "Schedule an email")

The message scheduler is the same for sending emails, text messages, push notificatons, social media posts and more. [Read more about using the scheduler](/campaigns/schedules).

### Send a Single Email<a name="single"></a>
To send a single email to a contact without scheduling the email and to bypass [sending rules](#send-rules) navigate to All Emails to browse the list of all published emails.

Click on the options menu of the email to send and select Send Email.

![Send single email](https://docs.dailystory.com/articles/emails/emails-25.png "Send single email")

This will open a popup. Select the contact to send the email to and click send.

## Email Sending Rules and Guardrails<a name="send-rules"></a>
DailyStory enforces rules when sending emails. These rules are in place to help you effectively communicate and ensure simple mistakes are avoided.

### A recipient is only sent an email once
When sending emails through automation or through the scheduler, DailyStory will ensure that a recipient will only receive your email once.

What this means is that an email can be scheduled repeatedly or sent again through a workflow without any concern of over-sending the same email. If the recipient was previously sent the email, they will not be sent the email again.

If a recipient asks to be resent the email, [send a single email](#single).

### Contact status must be Active
[Contacts](https://docs.dailystory.com/contacts/) whose status is not Active will not be sent emails.

### Lead status must be Active or Nurturing 
[Leads](https://docs.dailystory.com/leads/), Contacts within a campaign, whose status is not Active or Nurturing will not be sent emails.

### Contact must be Opted In
[Contacts](https://docs.dailystory.com/contacts/) who are marked as do not contact or have opted out of emails will not be sent emails.

## Import/Export an Email<a name="export"></a>
Emails created in DailyStory may be exported and imported. This enables customers to easily share emails between tenants in a secure manner.

> Exported emails are encrypted files.

### Export an Email
To export an email select Export from the [Options menu](#options). This will export an encrypted file [Name of the Email].elmz.

### Import an Email
To import an email, navigate to Content > Emails. Using the side menu, select Import:

![Emails Menu](https://docs.dailystory.com/articles/emails/emails-14.gif "Email Menu")

This open a popup. Select a DailyStory exported email (file ends with .elmz). The email is imported and the Email Setting screen is shown.

## Email Merge Tags<a name="merge-tags"></a>
Content created for DailyStory emails including Title, Subject and Body of your messages support [personalization tags and scripts](https://docs.dailystory.com/personalization). Personalization is the recommeneded way to personalize email content.

However, DailyStory also supports Merge Tags, a simpler form of personalization supported in other email platforms. Merge Tags may be used in the subject and body of your email.

The table below lists the Merge Tags supported by DailyStory:

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

> Important, if an <code>\*|UNSUBSCRIBE|\*</code> merge tag is not found an unsubscribe link is automatically inserted at the end of the email. An unsubscribe header with this link is also included in the email - these are best practices to ensure the email is not flagged as SPAM.

Any merge tags used in the email that do not have a value are automatically removed.

For example if the <code>\*|FNAME|\*</code> merge tag was used, but the contact does not have a Firstname field this:	 <code>Hi \*|FNAME|\*</code> Becomes: <code>Hi</code>

Merge tags provide a simple way to personalize your email, but do have limitations. For more robust personalization of your [email use personalization templates](https://www.dailystory.com/features/personalized-email-marketing/#templating-in-your-personalized-email-marketing).

### Enabling Email Web View
A web view of your email enables people to click a link in your email and view the email in a web browser.

> By default web view is disabled and no web view is available for your email.

To enable a web view of your email first enable the web view by clicked the toggle button on the Advanced Options tab:
	
![Enable Web View](https://docs.dailystory.com/articles/emails/emails-13.png "Enable Web View")

Next, use the <code>\*|WEBVIEW|\*</code> merge tag to include a link in your email.

> Note, the <code>\*|WEBVIEW|\*</code> merge tag only inserts the URL.

Optionally use the preview link next to the web view toggle button to preview what the web view of your email looks like. It will be personalized using the [Test Contact](/reference#test-lead).

The web view of the email is unique to each recipient. If personalization or merge tags are used in the email people who view the link will see the personalized view.

## Technical Details
Below is some technical information about the email format and content that DailyStory adds to your email.

**Doc Type**

DailyStory will automatically set the DOCTYPE to instruct HTML parsers that the content in the email is XHTML 1.0 Transitional:

`<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">`

**Meta Tags**

DailyStory will set the viewport meta tag:

`<meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=0" name="viewport"&gt>`

DailyStory will set the Apple's message reformatting meta tag:

`<meta name="x-apple-disable-message-reformatting">`

DailyStory will set the Microsoft's IE Edge meta tag:

`<meta http-equiv="X-UA-Compatible" content="IE=edge">`

DailyStory will set the meta tag to disable address recognition:

`<meta content="address=no" name="format-detection">`

DailyStory will set the meta tag to disable date recognition:

`<meta content="date=no" name="format-detection">`

DailyStory will set the meta tag to disable telephone recognition:

`<meta content="telephone=no" name="format-detection">`

DailyStory will set the meta tag to identify the content at HTML:

`<meta http-equiv="Content-Type" content="text/html; charset=utf-8">`

## Frequently Asked Questions<a name="faq"></a>
Below are some frequently asked questions about Emails.

## Why do emails look different across email clients?<a name="email-clients"></a>
The majority of modern email clients use a web browser as the rendering engine, i.e. to parse and interpret the HTML in the email. Unfortunately Microsoft Outlook uses Microsoft Word as the rendering engine. Microsoft Word's support for HTML is limited and some email elements may look slightly different in Outlook vs. Gmail. For example, buttons lose shading and some rounded styling aspects in Outlook.

## What email addresses are ignored?<a name="ignored-email-addresses"></a>
For testing and demonstration purposes you can use recipient addresses ending in <code>@test.com</code> and <code>@example.com</code>. These email addresses do not count towards your license limits and these emails will never be sent.

If you want to test sending emails, such as running a test lead through a workflow, we recommend using a disposable email address such as <a href="http://www.fakemailgenerator.com/" rel="noopener noreferrer">Fake Mail Generator</a>.

### What is an email preheader?<a name="faq-preheader"></a>
The majority of email clients provide a snippet of text to preview the contents of an email in your inbox. This enables you to quickly scan your inbox and decide if you want read, save, or archive the email.

This inbox preview text can be set using an [email preheader](https://www.dailystory.com/blog/email-preheader-improve-open-rates/).

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

### Does DailyStory support Merge Tags?<a name="faq-merge-tags"></a>
Yes. See [Email Merge Tags](#merge-tags) for more details. However, [personalization tags and scripts](https://docs.dailystory.com/personalization) is the recommeneded way to personalize email content.

### What happens if an email bounces?<a name="faq-bounce"></a>
Emails can [soft bounce](#faq-soft-bounce) or hard bounce. Hard bounces fail permanently and the [Contact's](/contacts) status is changed to Bounced.

### What is a soft bounce?<a name="faq-soft-bounce"></a>
A soft bounce occurs when the recipients email server temporarily is unable to receive the email. Such as when the mailbox is full.

### Will DailyStory try and resend soft bounces?<a name="faq-resend"></a>
Yes.  DailyStory will retry to send a soft bounced email up to 5 times over the next 24 hours. Afterwards, if the email is still undeliverable the [Contact's](/contacts) status is set to Bounced.