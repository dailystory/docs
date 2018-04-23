{
title: 'Paid Search Tracking Links',
description: 'Manage, forecast and budget paid search campaigns to understand and increase campaign conversion rates.'
}
# DailyStory Paid Search Tracking Links
DailyStory Paid Search is similar to DailyStory [Tracking Links](/link-tracking/). It enables you to track how link clicks convert visitors into customers. 

Paid Search links offer two differences from standard Tracking Links:

* **Budget Management** proide the approximate budget for your ads and DailyStory will calculate the cost per-qualified customer.
* **Keyword tracking** the ability to track the keyword a visitor converted on.

> Paid Search Tracking Links include tracking templates for both Google AdWords and Microsoft Bing Ads. Using these tracking templates you get the ability to track the keywords, device type and other information.

## Setting up DailyStory Paid Search with Google Ads
To create a new Paid Search Tracking Link go to Acquisition > Paid Search and follow the steps below.

<ol class="step"><li value="1">Create a new Paid Search Tracking Link</li></ol>

Create a new Paid Search Tracking Link by setting a friendly name, selecting a campaign, setting the URL you want to send the user to and optionally setting a monthly budget.

![Create Paid Search Tracking Link](/articles/aquisition/paid-search-01.png "Create Paid Search Tracking Link")

> You can also add UTM codes directly to your Destination URL or add/edit UTM codes from the Google Analytics tab.

Finally, Save the new Paid Search Tracking Link.

<ol class="step"><li value="2">Copy Tracking Link URLs</li></ol>

A Paid Search Tracking Link provides 3 URLs that you can use.

1. **Tracking Link URL** similar to a [Tracking Link](/link-tracking/) you can use this URL anywhere to track visitor conversions from ads.
2. **Google AdWords Tracking Template** a special tracking link for Google AdWords that adds keyword and device data from Google AdWords.
3. **Bing Ads Tracking Template** a special tracking link for Google AdWords that adds keyword and device data from Bing Ads.

## Tracking Link URL
The Tracking Link URL is a URL that you can use to track link clicks from any ad campaign or activity other than Google AdWords or Bing Ads.

For example, if you are running a Facebook Ad campaign, use the Tracking Link URL.

![Tracking Link URL](/articles/aquisition/paid-search-02.png "Tracking Link URL")

## Google AdWords Tracking Template
The Google AdWord Tracking Template is a URL specific to Google AdWords and enables DailyStory to capture additional information.

![Google AdWords Tracking Template](/articles/aquisition/paid-search-03.png "Google AdWords Tracking Template")

### Using the Google AdWords Tracking Template
To use the Google AdWords Tracking Template, copy the Google AdWords Tracking Template URL from DailyStory and then login to your Google AdWords account.

After signing in to Google AdWords navigate to Ads & extensions and edit an ad.

![Google AdWords Edit Ad](/articles/aquisition/paid-search-04.png "Google AdWords Edit Ad")

Next, click the arrow in the top-right of the screen.

![Google AdWords Edit Ad](/articles/aquisition/paid-search-05.png "Google AdWords Edit Ad")

This gives you an expanded view of the editor and also enables you to set additional Ad URL options.

Paste the Google AdWords Tracking URL copied from DailyStory into the Tracking template.

![Google AdWords Edit Ad](/articles/aquisition/paid-search-06.png "Google AdWords Edit Ad")

Next, set the Custom parameter <code>_adgroup</code> to the name of your Ad group in Google AdWords.

Your ad in Google AdWords is now configured to enable DailyStory to track clicks.