---
layout: _ArticleLayout
title: Web Forms
description: Web forms are used to collect information about your visitors.
---
# What is a DailyStory Web Form?
DailyStory enables you to quickly and easily create web forms that can be shown on your website, in our mobile application, a DailyStory landing page, or elsewhere using the DailyStory API.

Creating new web forms and editing existing webforms can be found by:

* Signing in to your DailyStory account
* Navigating to Acquisition > Web Forms	
	
![DailyStory Web Form](/articles/acquisition/web-forms/webforms-01.png "DailyStory Web Form")

This opens the All Web Forms list which shows a list of all web forms. Clicking on a web form will open the Edit Web Form Designer.

To create a new web form, click <code>+ New Web Form</code>

## Create a Web Form
When the <code>+ New Web Form</code> button is clicked the Create New Web Form designer is opened.

The first step is to select a campaign that the web form is associated with: 

![DailyStory Web Form](/articles/acquisition/web-forms/webforms-02.png "DailyStory Web Form")

This ensures that all leads or customers that complete this web form are associated with the right campaign. 

> By associating the web form with a campaign, the campaign will be given the attribution for the lead or customer conversion.

Once the campaign is selected the Web Form Designer is available:
	
![DailyStory Web Form Designer](/articles/acquisition/web-forms/webforms-03.png "DailyStory Web Form Designer")
	
## Web Form Designer	
The Web Form Designer enables you to create or edit an existing web form. Each web form requires:
	
* **A name** - a friendly name for the web form, such as Contact Us.
* **A destination URL** - where the form should send the browser once the form is completed.

The web form itself can have multiple form items, but the email address field is required and cannot be removed.

> If you attempt to remove the Email address form item an message will be shown that this form item is required and cannot be removed.

### Form Options
The Form Options section enable you to change some optional settings for the web form.

**Call to Action**
The Call to Action enables you to change the text shown on the call to action button for the web form. By default this is set to <code>Submit</code>.

If you would like the call to action to be something else, such as <code>Yes, please follow-up</code>, simply enter that text here.

** Form Layout**
The Form Layout option provides you with the ability to control some layout control of the web form. While the main styling of the web form is done with CSS, you can select:
	
* Display form labels - form labels (text above the form field) will be shown.
* Hide form labels - form labels (text above the form field) will not be shown.

> While displaying or not displaying form labels can also be controlled through CSS, this setting determines if DailyStory renders the HTML itself.

**Use reCAPTCHA**
If [reCAPTCHA integration](/integrations/recaptcha) is enabled 