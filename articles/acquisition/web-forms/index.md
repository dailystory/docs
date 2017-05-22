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

### Add / Edit Form Items
The Web Form Designer provides a simple preview of what your final web form will look like.

> This does not take into consideration any CSS applies to your web form.

Form items can be added, edited, removed and reordered using the designer.

#### Add Web Form Item
To add a web form item, click the drop down to select the type of form item to add. For example, to add a new textbox field click the Form item drop down and select textbox:

![Add form item](/articles/acquisition/web-forms/webforms-05.png "Add form item")

Next, a new form is shown

##### Textbox and Textarea
When Textbox or Textarea is selected the following options are availabe:

![Textarea form](/articles/acquisition/web-forms/webforms-06.png "Textarea form")

* Form label - this is the text shown with the form field
* Form placeholder - this is helpful text shown within the form field
* Lead field mapped to - the lead field in DailyStory to map the entered value to
* Make this required - prevents the form from being submitted unless this field is completed

Let's look an example: adding a new required form field for phone number:

![Add phone number](/articles/acquisition/web-forms/webforms-07.png "Add phone number")	

Next, we'll click 'Add form item' and this new field will be shown in the live preview:
	
![Add phone number form](/articles/acquisition/web-forms/webforms-08.png "Add phone number form")	

##### Dropdown list
DailyStory forms also support drop down lists so you can pre-define the values to be selected:
	
![Add drop down](/articles/acquisition/web-forms/webforms-09.png "Add drop down")	

> Unlike the textbox and textarea form items, there is not an option to set a form placeholder.

Drop down choices are set by entering a single option on each line. For example, if you want to ask the user to select their job title from a pre-defined list you can enter a single choice on each line. If you want to use a specific value different from the text use a comma (with no spaces):
	
![Drop down example](/articles/acquisition/web-forms/webforms-10.png "Drop down example")	

#### Edit Web Form Item
Editing a web form item is simple. Just click on the fom item to edit. It will turn yellow and the form item are displayed to the right.

![Edit form item](/articles/acquisition/web-forms/webforms-11.png "Edit form item")	

Click Update form item to save any changes and you will see this immediately reflected in the Live Preview.

#### Delete Web Form Item
Deleting a web form item is similar to editing. The only difference is that you click the Remove form item button.

### Form Options
The Form Options section enable you to change some optional settings for the web form.

#### Call to Action
The Call to Action enables you to change the text shown on the call to action button for the web form. By default this is set to <code>Submit</code>.

If you would like the call to action to be something else, such as <code>Yes, please follow-up</code>, simply enter that text here.

#### Form Layout
The Form Layout option provides you with the ability to control some layout control of the web form. While the main styling of the web form is done with CSS, you can select:
	
* Display form labels - form labels (text above the form field) will be shown.
* Hide form labels - form labels (text above the form field) will not be shown.

> While displaying or not displaying form labels can also be controlled through CSS, this setting determines if DailyStory renders the HTML itself.

#### Use reCAPTCHA
If [reCAPTCHA integration](/integrations/recaptcha) is an enabled integration you can add reCAPTCHA support to your web form.

> Provided by Google, reCAPTCHA is a free service that protects your website from spam and abuse by adding a simple test to your web or mobile experience.

The screen shot below shows an example form that includes reCAPTCHA:

![Web Form with reCAPTCHA](/articles/acquisition/web-forms/webforms-04.png "Web Form with reCAPTCHA")

### Unique Id
Once a web form is saved, or when it is edited, some additional properties about the webform are availabe. The Unique Id provides access to an id that uniquely identifies the form. This is used in the DailyStory APIs and for integrations such as [WordPress](/articles/integrations/wordpress).
	
![Web Form Unique Id](/articles/acquisition/web-forms/webforms-12.png "Web Form Unique Id")
	
