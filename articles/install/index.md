{
	title: 'DailyStory QuickStart: Your Guide to Getting Started with DailyStory',
	description: 'The DailyStory quickstart is a guide designed for new customers or users to help them get started.'
}
# Installing the DailyStory Tracking Tag
The DailyStory tracking tag, also called a tracking code, is a small piece of JavaScript that needs to be added to the <code>&lt;head&gt;</code> of all your web pages.

> The DailyStory tracking tag is similar to other tags, such as Google Analytics.

You can find the DailyStory tracking tag on the user drop down when you are signed in to DailyStory:
![Tracking Tag](/articles/install/install-01.png "Tracking Tag")

This will take you to the Account Settings > DailyStory Site ID and Tracking Code page:
![DailyStory Site ID and Tracking Code page](/articles/install/install-02.png "DailyStory Site ID and Tracking Code page")

> The Site ID, which is already included in the JavaScript tracking code, is a unique identifier that helps DailyStory know data is coming from your website.

The DailyStory JavaScript tracking code should be added to any pages within your website, community or landing pages where you want to enable DailyStory functionality. 

## Installation Guides
You can [install the tracking code manually](/install/manual) or follow one of our installation guides:

* [SquareSpace](/install/squarespace)
* [WordPress](/install/wordpress)

## Frequently Asked Questions
Below are some frequently asked questions about the DailyStory tracking tag.

### Where should I place the tag?
Place the tracking tag in the <code>&lt;head&gt;</code> section of all pages in your website as well as any landing pages. It's important that the tracking tag is available on any pages people may visit.

### How does the tracking tag work?
The tracking tag serves several purposes:
* Identifies and captures visits to build customer journey data
* Loads the DailyStory JavaScript API
* Enables integration with your website's forms
* Tracks incoming links to your website

### Does the tracking tag require JQuery?
No, the tracking tag does not require any other JavaScript libraries.

### Does the tracking tag slow down my web page?
No, the trackkng tag will not slow down your web page or interfere with loading pages in your website. The tracking tag is designed to load after your web page loads.