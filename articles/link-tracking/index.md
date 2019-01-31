{
	title: 'Link Management',
	description: 'DailyStory link management enable you to measure the relationship between marketing activities and the results generated from those activities.'
}
# DailyStory Tracking Links
Tracking Links are part of DailyStory's Link Management tools. These tools enable you to publish and share links to important content and measure their click-through performance.

The service is similar to other link management platforms such as [https://bit.ly](https://bit.ly). However, unlike stand alone link management tools, DailyStory's Tracking Links are integrated into the overall marketing and sales funnel. 

<iframe src="https://player.vimeo.com/video/314488961" width="640" height="480" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

> You do not need to create tracking links for email, text messages, social media, push notifications and any other content DailyStory sends to your contacts. This is done automatically through DailyStory's Link Management tools.

This guide provides a list of resources to help you get started with Tracking Links.

**Create and Edit a Tracking Link**

* [Create a Tracking Link](#create-a-tracking-link)
* [Test a Tracking Link](#test-a-tracking-link)
* [Edit a Tracking Link](#edit-a-tracking-link)

**Advanced Tracking Link Options**

* [Tracking Ad Clicks](#tracking-ad-clicks)
* [Integrate with Google Analytics](#integrate-with-google-analytics)
* [Advanced Options](#advanced-options)

**Reporting and Metrics**

* [Conversion Tracking](#conversion-tracking)
* [Click Tracking](#click-tracking)

**Frequently Asked Questions**

* [I already have a Link Management solution - can I integrate with DailyStory?](#i-use-another-link-management-platform-can-dailystory-integrate)
* [Why do my click metrics show no clicks?](#my-tracking-link-isnt-getting-any-clicks)
* [Do I need to create Tracking Links for emails or text messages I send through DailyStory?](#do-i-need-to-create-tracking-links-for-my-emails-or-text-message)
* [How does DailyStory auto-detect if the Tracking Tag exists?](#how-does-dailystory-know-if-my-destination-url-is-running-the-daily)
* [What is a Unique Click vs. a Unique IP address?](#what-is-a-unique-click-vs-a-unique-ip-address)
* [Why should I setup my own subdomain for DailyStory?](#why-should-i-setup-my-own-subdomain-for-dailystory)
* [How secure is DailyStory's Tracking Link password?](#how-secure-is-the-password-on-my-tracking-link)
* [What happens when I delete a Tracking Link?](#what-happens-when-i-delete-a-tracking-link)
* [Can I archive a Tracking Link?](#im-no-longer-using-the-tracking-link-how-do-i-keep-the-metrics)
* [Can my Destination Link redirect to another redirect URL?](#can-my-destination-url-redirect-to-another-url)

## Create a Tracking Link
Creating a Tracking Link is simple. Navigate to Acquisition > Tracking Links. 

To create a Tracking Link either:

* Enter a URL and press return. 
* Click the `+` button.
* Click `+ Create` in the main Tracking Link menu.

The image below shows the first option:
	
![Create Tracking Link](/articles/link-tracking/linktracking-04.png "Create Tracking Link")

Choosing any of the three options to create a Tracking Link will open up the Tracking Link editor.
	
![Edit Tracking Link](/articles/link-tracking/linktracking-05.png "Edit Tracking Link")

If the Tracking Link editor was opened from the `+` button or the `+ Create` menu option, you will need to enter the Destination URL yourself.

> DailyStory will attempt to automatically set the name of your Tracking Link to the title of the page you are linking to. But some pages don't have titles and you may need to set this yourself.

Clicking "Create" in the editor will generate the Tracking URL. The Tracking URL is what you publish or share. When people click your Tracking URL they will be redirected to the Destination URL.	

Once the your Tracking Link is saved, the Tracking Link editor will switch from create to edit mode. In edit mode there are more options for how DailyStory manages your Tracking Link.

## Test a Tracking Link
Use the `Test URL` button to test the Tracking URL. This will open a new browser tab and automatically open the Tracking URL. 

The `Test URL` button adds the query string value `?__PREVIEWMODE=1` to the end of your Tracking URL. When this is included metrics for your Tracking URL are not counted.

> When you use your Tracking URL make sure to use the Tracking URL and not the URL created by the `Test URL` result.

## Edit a Tracking Link
The Tracking Link edit screen is similar to the create screen, but with a few additional options. 

> When you enter or change the Tracking URL, DailyStory will automatically fetch the URL set the Name of the Tracking Link to the title of the page and provide a preview of the page.

When editing your Tracking Link you may have seen the "More Options..." link. Clicking this will expand additional options you can use to configure your Tracking Link.

## Tracking Link Options
Creating a basic Tracking Link using DailyStory's Link Management tools is easy. And for the most people, this is all you need. But, for advanced digital marketers, DailyStory includes more advanced options to control how your link behaves.

Click `More Options...` in the Tracking Link editor to expand the additional options. The first thing you see under `More Options...` is Google Ads and Bing Ads options.

### Tracking Ad Clicks
DailyStory Link Management integrates with Google and Bing Ad platforms. This integration enables you to see which ads created new leads and the keywords associated with those leads.

Integration with either Google Ads or Bing Ads require the use of a special Tracking URL.

> To integrate with Google Ads or Bing Ads you must use the unique Tracking URLs for those services.

![Ad Link Tracking](/articles/link-tracking/linktracking-06.png "Ad Link Tracking")	

These are special Tracking URLs used with Google Ads and Bing Ads and enable DailyStory to recieve additiona detail. This includes: device information, keywords, ad groups and more.	

> If you are using [retargeting pixels](/link-tracking/what-is-retargeting-pixel) with your ads DailyStory Link Management will automatically include your Retargeting Pixel when redirecting visitors to your Destination URL.

While DailyStory does receive and provide reports on the keywords that attracted clicks, it can only report on the keywords associated with your ad.

For example, if your paid ad keyword included 'apple' and the search was 'apple watch guide' DailyStory will only receive the 'apple' keyword for reporting purposes. Thus, the more keywords and terms used in your ad, the more precise DailyStory's keyword reporting is.

#### Google Ads
Follow the instructions below to use your Tracking Link with Google Ads. Google Ads support a Tracking template that can be used for DailyStory Link Tracking.

<ol class="step"><li value="1">Create Google Ad</li></ol>
Create a Google Ads ad or edit an existing ad.

<ol class="step"><li value="2">Click + on Ad options</li></ol>
Click [+] on Ad URL options (advanced) as shown in the image below:

![Google Ads](/articles/link-tracking/linktracking-01.png "Google Ads")

<ol class="step"><li value="3">Copy/Paste Tracking Template URL</li></ol>
Copy/Paste the Google Ads Tracking Template URL into the Tracking template text box (highlighted in red) above.

<ol class="step"><li value="4">Save</li></ol>
Finally, save your Google Ads ad. You can also test the links too.

#### Bing Ads
Follow the instructions below to use your Tracking Link with Bing Ads. Bing Ads support a Final URL that can be used for DailyStory Redirect Link Tracking.

<ol class="step"><li value="1">Create Bing Ad</li></ol>
Create a new Bing Ads ad or edit an existing ad.

<ol class="step"><li value="2">Set Final URL</li></ol>
When editing the ad, select Final URL (recommended) as shown in the image below:

![Bing Ads](/articles/link-tracking/linktracking-02.png "Bing Ads")

<ol class="step"><li value="3">Copy/Paste Tracking Template URL</li></ol>
Copy/Paste the Bing Ads Final URL into the text box (highlighted in red) above.

<ol class="step"><li value="4">Save</li></ol>
Finally, save your Bing Ads ad. You can also test the links too.

### Integrate with Google Analytics
Using Google Analytics integration, DailyStory Link Management can pass additional Google Analytics data with your Destination URL.

![Google Analytics](/articles/link-tracking/linktracking-07.png "Google Analytics")

Configuring Google Analytics enables you to pass additional campaign details to Google Analytics and DailyStory.

> Consider setting your Google Analytics campaign name to the name of your DailyStory campaign to more easily see how customers flow through your website.

DailyStory will automatically append this information to your Destination URL.

In addition to Google Analytics data, you can append any additional data in the query string to your Tracking URL. DailyStory Link Management will automatically forward the query string data to your Destination URL. This is handy if you have special values that you want to capture.

### Advanced Options
DailyStory Link Management provides several advanced options for managing your links.
	
![Additional Options](/articles/link-tracking/linktracking-08.png "Additional Options")

#### Web page or file
By default, DailyStory Link Management presumes the Destination URL is a web page. If it is not a web page, but is a file (such as a PDF), you can tell DailyStory's Link Management to treat the results from the Tracking URL as a file. Doing so weill download the file to the client's browser by setting the appropriate HTTP headers.

#### Alternative URL
If your Tracking URL expires or a password is invalid, DailyStory Link Management will redirect people to this URL. If you do not provide an Alternative URL and the URL is no longer valid, visitors will be redirected to a generic DailyStory URL indicating that the content is no longer available.

> It's easy to create an Alternative URL by creating a new [Landing Page](/pages/) in DailyStory and using to URL to your Landing Page as the Alternative URL.

#### Redirect Type
The Redirect Type Temporary (the default) sends an HTTP 302 status code when DailyStory Link Management redirects to your Destination URL. Setting the Redirect Type to Permanent sends an HTTP 301 status code.

> It is recommended that the Redirect Type is set to Temporary unless you fully understand why a HTTP 301 is needed.

#### Password
Set a password that will be required before DailyStory Link Management redirect to your Destination URL. This is useful if you have content you wish to share, such as a PDF, but want to require people to authenticate prior to accessing it.

#### Maximum Clicks
This option allows you to set the maximum number of clicks allowed for the Tracking URL. Once this limit is reached, visitors will be redirected to your Alternative URL or will receive a generic DailyStory URL indicating that the content is no longer available.

#### Expiration Date
This option allows you to set a date after which the Tracking URL expires. Once this date is reached, visitors will be redirected to your Alternative URL or will receive a generic DailyStory URL indicating that the content is no longer available. 

## Tracking Link Metrics and Reporting
DailyStory Link Management automatically tracks metrics, such as unique clicks, on your links. But the measurements are slightly different when Link Management detects the DailyStory tag.

### Conversion Tracking
If your tracking link redirects to a page hosting the DailyStory [tracking code](/install), such as your website or a DailyStory [landing page](/pages/), DailyStory Link Management will track and report:

* Total Clicks
* Unique Clicks
* Converted Leads 
* Accessing device (mobile, tablet or desktop)
* Keywords (when integrated with [Google Ads or Bind Ads](#tracking-ad-clicks))

Anonymous visitors that convert on [Web Form](/acquisition/web-forms/), [Magic Form](/acquisition/magic-forms/), [Popup](/acquisition/popups/) or through the [API](/api/) are shown in the Contact's and Lead's activity report. Also included is the link they originally clicked on:
	
![Tracking Link Conversion](/articles/link-tracking/linktracking-03.png "Tracking Link Conversion")

> If you are using [retargeting pixels](/link-tracking/what-is-retargeting-pixel) DailyStory Link Management will automatically include your Retargeting Pixel when redirecting visitors to your Destination URL.

### Click Tracking
If your tracking link redirects to a page that is not hosting the DailyStory [tracking code](/install), such as an article on CNN, DailyStory Link Management will track the total click through and unique click through based on the visitor's IP address.

It's important to note the difference between conversion tracking and click tracking metrics. Conversion Tracking reporting on inbound links (content you own) whereas Click Tracking reports on outbound links (content you don't own). Conversion Tracking is much more accurate because individual visitors are tracked vs. unique IP addresses.

#### Better Click Tracking
While Click Tracking doesn't provide the same benefits as conversion tracking, there are some advanced configuration options available to improve your metrics.

1. Retargeting Pixels - DailyStory will include your [retargeting pixels](/link-tracking/what-is-retargeting-pixel). 
2. Add a subdomain - Request to add your own subdomain to DailyStory. This will allow us to write the tracking code to visitor's browser even if Link Management redirects them to an outbound link where the DailyStory tracking tag is not running.

## Frequently Asked Questions
Below are some frequently asked questions about Tracking Links.

### I use another Link Management platform, can DailyStory integrate with it?
No, we currently do not integrate with other Link Management solutions. DailyStory's Link Management is part of the DailyStory platform and is designed to bring together many different tools into a single integrated solution. In the future we may consider integrating with other Link Management platforms. We also [do not recommend](#can-my-destination-url-redirect-to-another-url) using a DailyStory Tracking Link to point to a Destination URL that goes through another Link Management platform.

### My Tracking Link isn't getting any clicks
There is a 15-20 minute delay from when a Tracking Link is clicked until the metrics start showing up. However, if you still aren't seeing any metrics it may be because the Tracking Link isn't setup correctly. First check that the Tracking Link works using the [Test Tracking Link](#test-a-tracking-link) button. If the link is redirecting properly to your Destination URL, next check that the link you are sharing doesn't include the `?__PREVIEWMODE=1`. This is a special instruction to tell DailyStory Link Management not to record metrics. Finally, if your Tracking Link still isn't working, please [Contact Us](https://www.dailystory.com/contact-us). We'd be happy to help.

### How does DailyStory know if my Destination URL is running the DailyStory Tracking Tag?
When you save your Tracking Link, DailyStory Link Management will validate your Destination URL and check if the DailyStory Tracking Tag is installed. There is nothing you need to do.

### Do I need to create tracking links for my emails or text messages?
No, just create content in DailyStory and add links to whatever content you want. DailyStory Link Management will update your content and replace your links with Tracking Links before the content is sent.

### What is a Unique Click vs. a unique IP address?
When a link is redirected to a URL running the DailyStory Tracking Tag, the Tracking Tag will receive information about the Tracking Link as a Unique Click and use this when it records the visit to the page. Later these visits, and link clicks, are aggregated into metrics for reports. This is distinct from a Unique IP address - Link Management receives the redirect request, but if the Destination URL is not running the DailyStory Tracking Tag a Unique Click cannot be recorded.

### Why should I setup my own subdomain for DailyStory?
When someone clicks on your Tracking Link, DailyStory Link Management receives the request to our domain (https://dlystr.io). This is a special short-code domain setup for our customers to use. However, requests that use this short-code URL and then redirect to a URL that is not running the DailyStory tracking tag can only [track clicks not conversions](#click-tracking). If you provide your own URL for DailyStory to use that shares your domain, DailyStory can write a tracking cookie for your domain.

### How secure is the password on my Tracking Link?
Requiring a [password](#password) before DailyStory Link Management redirects to your Destination URL does not protect your content if the Destination URL is shared. If you require security for a file or page you wish to share to prevent access to the resource at the Destination URL, then you should consider more secure options.

### What happens when I delete a Tracking Link?
When you delete a Tracking Link, the Tracking Link may continue to work, but will soon be unavailable and future clicks will be redirected to a generic DailyStory page indicating that the link is no longer available. Deleted links are moved to the Trash and can be recovered. However, after several days the Tracking Link and all metrics associated with it will be permanently deleted.

### I'm no longer using the Tracking Link, how do I keep the metrics?
If you are no longer using a Tracking Link, but wish to retain metrics for the Tracking Link, you can Archive the Tracking Link. Tracking Links that are archived are no longer usable, but are not deleted.

### Can my Destination URL redirect to another redirect URL?
Generally speaking, multiple redirects is considered bad and you risk Google, and other search engines, penalizing your links. We recommend that any Destination URL that DailyStory Link Management redirects to is the URL you want your visitors to end up at.

