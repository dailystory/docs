{
	title: 'Link Tracking',
	description: 'Link tracking enables marketers to measure the relationship between marketing activities and the results generated from those activities.'
}
# What is a Tracking Link?
A Tracking Link enables you to measure the relationship between activities and the results generated from those activities. 

The service is similar to other link management platforms such as [https://bit.ly](https://bit.ly). However, unlike stand alone link management tools, DailyStory's Tracking Links are integrated into the overall marketing and sales funnel. 

## Creating a Tracking Link
Creating a Tracking Link is simple. Just navigate to Tracking Links and either enter a URL or click the + button:
	
![Create Tracking Link](/articles/link-tracking/linktracking-04.png "Create Tracking Link")

This will open up the Tracking Link editor:
	
![Edit Tracking Link](/articles/link-tracking/linktracking-05.png "Edit Tracking Link")

If you entered a URL, DailyStory will automatically fetch the URL set the Name of the Tracking Link to the title of the page and provide a preview of the page.

Clicking "Create" will then generate the Tracking URL. The Tracking URL is what you publish. When people click your Tracking URL they will be redirected to the Destination URL.	

## Tracking Link Metrics
DailyStory automatically tracks metrics on your links, but the measurements are slightly different:

### Conversion Tracking
If your tracking link redirects to a page hosting the DailyStory [tracking code](/install), such as your website or a DailyStory [landing page](/pages/), we'll track unique visitors that get tagged with a DailyStory tracking id. 

If these visitors convert you'll be able to see the conversion in your activity report along with the link they originally clicked on:
	
![Tracking Link Conversion](/articles/link-tracking/linktracking-03.png "Tracking Link Conversion")

> If you are using [retargeting pixels](/link-tracking/what-is-retargeting-pixel) DailyStory will automatically include these.

### Click Tracking
If your tracking link redirects to a page that is not hosting the DailyStory [tracking code](/install), such as an article on CNN, we'll track the total click through and unique click through based on the visitor's IP address.

#### Better Click Tracking
While Click Tracking doesn't provide the same benefits as conversion tracking, there are some advanced configuration options available:

1. Retargeting Pixels - DailyStory will still include [retargeting pixels](/link-tracking/what-is-retargeting-pixel).
2. Add a subdomain - You can add your own subdomain to DailyStory and this will allow us to write the tracking code to visitors even if they aren't going to a page on your site.

## More Options
When editing your Tracking Link you may have seen the "More Options..." link. Clicking this will expand additional options you can use to configure your Tracking Link.

## Tracking Ad Clicks
The first thing you see under "More Options..." is unique URLs for Google Ads and Bing Ads:

![Ad Link Tracking](/articles/link-tracking/linktracking-06.png "Ad Link Tracking")	

These are special URLs used with Google Ads and Bing Ads that will enable DailyStory to additionally receive details, such as the keywords people clicked on.	

### Google Ads
Follow the instructions below to use your tracking link with Google Ads. Google Ads support a Tracking template that can be used for DailyStory Link Tracking.

<ol class="step"><li value="1">Create Google Ad</li></ol>
Create a Google Ads ad or edit an existing ad.

<ol class="step"><li value="2">Click + on Ad options</li></ol>
Click [+] on Ad URL options (advanced) as shown in the image below:

![Google Ads](/articles/link-tracking/linktracking-01.png "Google Ads")

<ol class="step"><li value="3">Copy/Paste Tracking Template URL</li></ol>
Copy/Paste the Google Ads Tracking Template URL into the Tracking template text box (highlighted in red) above.

<ol class="step"><li value="4">Save</li></ol>
Finally, save your Google Ads ad. You can also test the links too.

### Bing Ads
Follow the instructions below to use your redirect link with Bing Ads. Bing Ads support a Final URL that can be used for DailyStory Redirect Link Tracking.

<ol class="step"><li value="1">Create Bing Ad</li></ol>
Create a new Bing Ads ad or edit an existing ad.

<ol class="step"><li value="2">Set Final URL</li></ol>
When editing the ad, select Final URL (recommended) as shown in the image below:

![Bing Ads](/articles/link-tracking/linktracking-02.png "Bing Ads")

<ol class="step"><li value="3">Copy/Paste Tracking Template URL</li></ol>
Copy/Paste the Bing Ads Final URL into the text box (highlighted in red) above.

<ol class="step"><li value="4">Save</li></ol>
Finally, save your Bing Ads ad. You can also test the links too.

## Google Analytics
If you want to pass additional data with your Destination URL, such as information used by Google Analytics, you can configure that here.

![Google Analytics](/articles/link-tracking/linktracking-07.png "Google Analytics")

DailyStory will automatically append this information to your Destination URL.

> An advanced tip: you can append query string data to your Tracking Link and DailyStory will forward the query string data to your Destination URL. This is handy if you have special values that you want to capture.

## Additional Options
If you are slighly more advanced with your knowledge of Tracking Links, we provide some handy advanced options:
	
![Additional Options](/articles/link-tracking/linktracking-08.png "Additional Options")

* **Web page or file** - we'll set the appropriate HTTP headers for you.
* **Alternative URL** - if your link expires or the password is invalid, we can redirect people here.
* **Redirect Type** - useful for search engines and let's them know if this is a permanent redirect or a temporary redirect.
* **Password** - enter this password to get redirected to the Destination URL.
* **Maximum Clicks** - limit how many times we'll redirect to your Destination URL.
* **Expiration Date** - after this date we'll redirect to the Alternative URL. 

## Frequently Asked Questions
Below are some frequently asked questions about Tracking Links.

### How does DailyStory know if my link is pointing to a page hosting the DailyStory tracking code?
It's important to know this so we know which metrics to track. It's some built in magic ... just kidding, when we save your tracking link we check the URL you want the tracking link to redirect to and look for our tracking code.

