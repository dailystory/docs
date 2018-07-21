{
	title: 'Popups',
	description: 'Popups can be shown automatically or using the API.'
}
# DailyStory Popups
A [DailyStory Popup](https://www.dailystory.com/features/welcome-exit-offers/) enables you to display a popup window in a web or mobile experiece.

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F_uzD2F7RaLo%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D_uzD2F7RaLo&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2F_uzD2F7RaLo%2Fhqdefault.jpg&key=internal&type=text%2Fhtml&schema=youtube" width="500" height="281" scrolling="no" frameborder="0" allowfullscreen></iframe>

Popups can be shown on specific pages, configured to automatically show after a certain amount of time has passed, when the visitor first arrives, or if the visitor is leaving the site.

![DailyStory Popup](https://www.dailystory.com/files/imgs/welcome-exit-offers-sample.jpg "DailyStory Popup")

[Read more about the benefits of DailyStory Popups at dailystory.com](https://www.dailystory.com/features/welcome-exit-offers/).

## Creating and Editing a Popup
To creae a new popup go to Acquisition > Popups. This will show you a list of all the existing popups. You can edit a popup by clicking on it and you can create a new popup by clicking the + New Popup button:
	
![All Popups](/articles/acquisition/popups/popup-06.png "All Popups")

Clicking either will open the popup editor:

![Popup Editor](https://www.dailystory.com/files/imgs/welcome-exit-offers-create.jpg "Popup Editor")

The popup editor provides a live preview of your popup. You can enter a title, body, call to action button text, call to action url, close/cancel button text and select a background image. All of these settings will be immediately refelected in the live preview window.

Some fields have additional options that can be configured. You can also add form fields for name and email address. This is useful if you provide an offer such as a newsletter signup or download.

### Popup Interactions

A popup typically has 2 types of interactions:

* **Call to Action** - the Call to Action (CTA) can complete a form, such as a newsletter signup or navigate to another page. This is the primary objective of the popup offer: to get the person viewing the popup to take some kind of action.
* **Close / Dismiss** - the Close or Dismiss button closes the popup and may navigate the user to another page or simply disappear.

More advanced popups introduce nuances for dismissing the offer:

* Close, but remind me later - the visitor dismisses the popup but indicates that they would like to receive the popup again in the future.
* Close and ignore - this enables the visitor to dismiss the popup and to never show it again.

These types of popup interactions are important because DailyStory tracks these choices and enables you to test which converts best.

### Metrics Tracked for Popups

DailyStory tracks several metrics related to popups:

* **Impressions** - the number of times the popup is shown to visitors.
* **Ignores** - the number of times no interaction with the popup takes place.
* **Call to Action click** - the number of times the main popup call to action is clicked.
* **Dismiss click** - the number of times the dismiss button is clicked.

These metrics are shown in the reports for your popup.

### Configuring Title Options	
The Title Options enable you to set the font color and font size of the title text:
	
![Title Options](/articles/acquisition/popups/popup-07.png "Title Options")

> These options configure CSS settings for <code>#ds_pop h1</code>

### Configuring Body Content	
Body content should be brief. You can use the return key to create line breaks in the content.
	
> The body content is wrapped in a &lt;p&gt; tag with &lt;br&gt; to handle line breaks. CSS settings for <code>#ds_pop .content p</code>

You can configure the text and background color of the body content in Background Options.

### Configuring Call to Action Button
The Call to Action button is the primary action you want viewers to take. When clicked, the call to action button can navigate to another URL or capture a name and email address (see Lead Capture Form below for more details).

The Call to Action Options enable you to configure the color/style of the call to action button:

![Call to Action Options](/articles/acquisition/popups/popup-08.png "Call to Action Options")

> The call to action button applies CSS settings for <code>#ds_pop a#ds_pop_action_button</code>

When the Call to Action button is clicked the popup will not be shown to this user again.

### Configuring Call to Action URL
The Call to Action URL is the URL to redirect the visitor to when the Call to Action button is clicked.

> If a Lead Capture Form is configured, the form will send the data entered into the form and then redirect to this URL.
	
### Configuring Close/Cancel Button
The Close/Cancel button is used to close the popup because the offer presented to the visitor is not of interest.

> By default, when the Close/Cancel button is clicked the popup will not be shown again to that visitor for one week. However, this can be configured.

![Close Cancel](/articles/acquisition/popups/popup-03.png "Close Cancel")

The Close/Cancel button options present three toggles:

* **Display button** - enabled by default, this determines if the Close/Cancel button is shown.
* **Display quick close** - enabled by default, this determines if the X in the upper-right corner is shown.
* **Easy ignore** - disabled by default, this allows clicking outside of the popup or pressing escape to close the popup.

> It is important to note that it is possible to configure the popup with no way to close except for the call to action.

In addition to the behavior toggles there are options for setting the button colors/style.

Finally, the Set Close/Cancel Options also enable you to configure how long to hide the popup after the close/cancel button is clicked. The recommendation is 1 week.

### Configuring Background
The Background Options enable you to set an image used in the background of the popup as well as the text and background colors:

![Background Options](/articles/acquisition/popups/popup-09.png "Background Options")

> The background color and image set CSS for <code>#ds_pop</code> and the background text color for <code>#ds_pop .content</code>

You can also provide a URL to your own image file or upload an image to DailyStory.

### Configuring Lead Capture Form
The Lead Capture Form enables you to capture visitor information and create new leads within a DailyStory campaign.

Popups are great for capturing visitors that read your blog and you can offer to sign them up for your newsletter.

![Lead Capture Form](/articles/acquisition/popups/popup-10.png "Lead Capture Form")

> Important - if you use the Lead Capture Form, the email address is required and the fullname is optional. You must also choose the campaign to assign new leads to.

### Advanced Options
The Advanced Options provide capabilities that customers can change, but are completely optional and typically not used.

![Advanced Options](/articles/acquisition/popups/popup-11.png "Advanced Options")

The Close Forever button is an additional behavior added to your popup that displays an additional button or link. Unlike the Close/Cancel button, the Close Forever button will not show the popup again to that user for one year.

You can additionally configure other automated behaviors of the popup.

The **Automatically display if no browser activity** will display the popup if the visitor has no activity for the specified time period. For example, if they open your page in a new tab or do something else, when they come back the popup will be displayed if the specified time has elapsed.

The **Minimum visitor time on site** controls the minimum amount of time the visitor must be on the website before the popup can be shown. This is useful if a visitor goes to your site and immediately leaves. It is designed to ensure that if a visitor stays longer than the specified time, they must be enagaged.

## Testing your Popup
Now that you've created a popup. You can test your popup to see what it will look like when shown to your website visitors.

On the bottom right of the popup editor you will see a button that says, "Test Popup".

![Test Popup](/articles/acquisition/popups/popup-12.png "Test Popup")

Clicking this button will open a new browser tab. After a 2 second delay your popup will be shown.

![Test Popup](/articles/acquisition/popups/popup-13.png "Test Popup")

Once you have verified that your popup looks like you expect you can close the popup tab.

## How do I enable a DailyStory Popup?
Popups are automatically shown on every page of your website or on specific pages, or paths, of your website. 

> Important - popups are never shown on your website until you select where they should be shown.

For example, you can create a popup that is only shown to visitors of your blog by using a path of <code>/blog/*</code>. 

By default a popup is double -ocked to prevent it from displaying on your site by accident.

1. There is a master enabled/disabled at the top of the popup designer. The popup will never be shown if this switch is set to off. 
![DailyStory Popup](/articles/acquisition/popups/popup-01.png "DailyStory Popup")

2. In addition to enabling the master enabled/disabled switch, you must select where the popup will be displayed.
![DailyStory Popup](/articles/acquisition/popups/popup-02.png "DailyStory Popup")

Configuring where to show the popup using the rules found in the popup designer are recommeneded. However, more advanced users can use DailyStory's JavaScript API to control exactly when a popup is shown.

## How to display a DailyStory Popup with the JavaScript API
Using the DailyStory JavaScript API you can display any DailyStory popups which you have enabled.

To use the JavaScript API to show a popup you will need the <code>id</code> of the enabled popup. The popup <code>id</code> is a numeric value, such as 35, and can be found in the URL when editing the popup in DailyStory:
	
<code>https://us-1.dailystory.com/Acquisition/EditExitIntent/35</code>

Before attempting to use the JavaScript API, first verify that the popup is in the Json file DailyStory creates for your account.

### The DailyStory Popup Json File
DailyStory's JavaScript API, initialized by the [DailyStory tag](/install), runs asynchronously after the page loads and does not interfere with your page rendering. It also asynchronously loads a JSON file, which is cached by the client browser.

DailyStory Popups are loaded from the data center specific URL of your DailyStory tenant. For example, a tenant in data center US-1 with the tenant id of 1a2b3c4d loads its JSON from:

<code>https://us-1.dailystory.com/ds/1a2b3c4d.json</code>

This file will include any DailyStory Popups that are enabled for the tenant as well as other DailyStory features you have enabled.

> Important: due to caching of the file, if you enable or change a popup in DailyStory it may take up to 20 minutes for changes to be available to your website.

## Showing a popup when the page loads
To show a popup when the page loads using the JavaScript API add the following script (replacing 35 with the numeric id of your popup).

<script type="syntaxhighlighter" class="brush: js">
window.addEventListener('ds_popup_ready', function(e) {
   Ds.Pop.showPopup('35');
});
</script>	

The DailyStory API uses browser events to call your code after DailyStory is loaded.

> Important: DailyStory loads all its files after the main page loads. This ensures that the user's content is displayed as quickly as possible.

## Show a specific popup offer when the visitor is leaving
To show a popup when the visitor is leaving your website using the JavaScript API, add the following script:

<script type="syntaxhighlighter" class="brush: js">
window.addEventListener('ds_popup_ready', function(e) {
	Ds.Pop.showPopupOnExit('35');
});
</script>