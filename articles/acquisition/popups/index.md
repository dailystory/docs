---
layout: _ArticleLayout
title: Popups
description: Popups can be shown automatically or using the API.
---
# What is a DailyStory Popup?
A DailyStory Popup enables you to display a popup window in a web or mobile experiece:

![DailyStory Popup](/articles/acquisition/popups/popup-04.png "DailyStory Popup")

Popups can be shown on specific pages and configured to automatically show after a certain amount of time has passed or if the visitor is leaving the site.	

## Creating and Editing a Popup
To creae a new popup go to Acquisition > Exit Intent. This will show you a list of all the existing popups. You can edit a popup by clicking on it and you can create a new popup by clicking the + New Exit Intent button:
	
![All Popups](/articles/acquisition/popups/popup-06.png "All Popups")

Clicking either will open the popup editor:

![Popup Editor](/articles/acquisition/popups/popup-05.png "Popup Editor")

The popup editor provides a live preview of your popup. You can enter a title, body, call to action button text, call to action url, close/cancel button text and select a background image. All of these settings will be immediately refelected in the live preview window.

Some fields have additional options that can be configured. You can also add form fields for name and email address. This is useful if you provide an offer such as a newsletter signup or download.

### Configuring Title Options	
The Title Options enable you to set the font color and font size of the title text:
	
![Title Options](/articles/acquisition/popups/popup-07.png "Title Options")

> These options configure CSS settings for <code>#ds_pop .content h1</code>

### Configuring Body Content	
Body content should be brief. You can use the return key to create line breaks in the content.
	
> The body content is wrapped in a <p> tag with <br> to handle line breaks. CSS settings for <code>#ds_pop .content p</code>

You can configure the text and background color of the body content in Background Options.

### Configuring Call to Action Button
The Call to Action button is the primary action you want viewers to take. When clicked, the call to action button can navigate to another URL or submit a lead capture form (see Lead Capture Web Form).

The Call to Action Options enable you to configure the color/style of the call to action button:

![Call to Action Options](/articles/acquisition/popups/popup-08.png "Call to Action Options")

> The call to action button applies CSS settings for <code>#ds_pop a#ds_pop_action_button</code>

### Configuring Call to Action URL
The Call to Action URL is the URL to redirect the visitor to when the Call to Action button is clicked.

> If a Lead Capture Web Form is configured the form will submit and then redirect to this URL.
	
### Configuring Close/Cancel Button
The Close/Cancel button is used to close the popup because the offer presented to the visitor is not of interest.

> By default, when the Close/Cancel button is clicked the popup will not be shown again to that visitor for one week.

![Close Cancel](/articles/acquisition/popups/popup-03.png "Close Cancel")

The Close/Cancel button options present three toggles:

* **Display button** - enabled by default, this determines if the Close/Cancel button is shown.
* **Display quick close** - enabled by default, this determines if the X in the upper-right corner is shown.
* **Easy ignore** - disabled by default, this allows clicking outside of the popup or pressing escape to close the pop-up.

> It is important to note that it is possible to configure the popup with no way to close except for the call to action.

In addition to the behavior toggles there are options for setting the button colors/style.

Finally, the Set Close/Cancel Options also enable you to configure how long to hide the popup after the close/cancel button is clicked. The recommendation is 1 week.

### Configuring Background
The Background Options enable you to set an image used in the background of the popup as well as the text and background colors:

![Background Options](/articles/acquisition/popups/popup-09.png "Background Options")

> The background color and image set CSS for <code>#ds_pop</code> and the background text color for <code>#ds_pop .content</code>

> You can provide a URL to your own image file or upload an image to DailyStory.

### Configuring Lead Capture Form
The Lead Capture Form enables use to capture visitor information and create new leads within a DailyStory campaign.

![Lead Capture Form](/articles/acquisition/popups/popup-10.png "Lead Capture Form")

> If you use the Lead Capture Form, the email address is required and the fullname is optional.

## How do I enable a DailyStory Popup?
Popups can automatically be shown on every page of your website or on specific pages, or paths, of your website. 

For example, you could create a popup that is only shown to visitors of your blog by using a path of <code>/blog/*</code>. 

> Note: In the example above, this assumes that all blog posts exist within that path.

By default a popup is double locked to prevent it from displaying on your site by accident.

1. There is a master enabled/disabled at the top of the popup designer. The popup will not be displayed if this switch is set to off. 
![DailyStory Popup](/articles/acquisition/popups/popup-01.png "DailyStory Popup")

2. In addition to enabling the master enabled/disabled switch, you must select where the popup will be displayed.
![DailyStory Popup](/articles/acquisition/popups/popup-02.png "DailyStory Popup")

## How to display a DailyStory Popup with the JavaScript API
Using the DailyStory JavaScript API you can force the display of any DailyStory popup that is enabled.

To use the JavaScript API to force a popup you will need the <code>id</code> of the enabled popup. The popup <code>id</code> is a numeric value, such as 35, and can be found in the URL when editing the popup in DailyStory:
	
<code>https://us-1.dailystory.com/Acquisition/EditExitIntent/35</code>

## The DailyStory Popup Json File
DailyStory's JavaScript API runs asynchronously after the page loads so it does not interfere with your page rendering. It also asynchronously loads several JSON files, which can be cached by the client browser.

DailyStory Popups are loaded from the data center specific URL of your DailyStory tenant. For example, a tenant in data center US-1 with the tenant id of 1a2b3c4d loads its JSON from:

<code>https://us-1.dailystory.com/ds/pp1a2b3c4d.json</code>

This file will include any DailyStory Popups that are enabled for the tenant.

> Important: due to caching of the file, if you enable a popup in DailyStory it may not be available immediately.

You can also find the <code>id</code> of each popup in the JSON file.

## Showing a popup when the page loads
To show a popup when the page loads using the JavaScript API, add the following script:

<script type="syntaxhighlighter" class="brush: js">
window.addEventListener('ds_popup_ready', function(e) {
   Ds.Pop.showPopup('35');
});
</script>	

The DailyStory API uses browser events to call your code after DailyStory is loaded. 

> Important: DailyStory loads all its files after the main page loads. This ensures that the user's content is displayed as quickly as possible.

## Showing a popup on exit intent
To show a popup when the visitor is leaving your website using the JavaScript API, add the following script:

<script type="syntaxhighlighter" class="brush: js">
window.addEventListener('ds_popup_ready', function(e) {
	Ds.Pop.showPopupOnExit('35');
});
</script>