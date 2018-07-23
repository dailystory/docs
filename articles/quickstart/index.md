{
	title: 'DailyStory Quick Start: Your Guide to Getting Started with DailyStory',
	description: 'The DailyStory quickstart is a guide designed for new customers to help them get started.'
}
# DailyStory Quick Start: Getting Started with DailyStory
Welcome to DailyStory! We put this guide together to help you get started using DailyStory.

## Technical Requirements
The good news is: you don't need a degree in computer science to start using DailyStory. And, you won't need a team to setup and manage DailyStory.

However, there are a few things you need to do to get the most out of DailyStory.

### Setting up the DailyStory tracking tag
The DailyStory tracking tag connects DailyStory and your website. It's required to use many of the features of DailyStory.

<ol class="step"><li value="1">Install the Tracking Tag</li></ol>
The tracking tag is a small piece of JavaScript that needs to be added to the <code>&lt;head&gt;</code> of all your pages.

Follow these instructions to [install the DailyStory tracking tag](/install). 

> The DailyStory tracking tag is similar to other tags, such as Google Analytics.

We have instructions for [installing the tracking tag manually](/install/manual) as well as using our [WordPress plugin](/install/wordpress).

[Tracking Tag Frequently Asked Questions](/install#Frequently-Asked-Questions)

### Optionally configure Email and a Domain
You can start using DailyStory without setting up email or a custom domain. Email will be sent on your behalf through DailyStory's email system and your pages and content will be hosted on DailyStory's domain.

People that receive your email will see the message as coming from:
	
`Anna Jones <anna@example.com> on behlaf of DailyStory`

Landing pages or other content hosted on DailyStory will look like:
	
`https://dlystr.io/Sample-landing-page?_UID=4933ca402181fcf4a5c94713daaa9921`

To configure your own email account and subdomain, please [follow the steps in our technical setup guide](/install/setup)

<ol class="step"><li value="2">Create a Campaign</li></ol>
Once you have the tracking tag setup, you'll want to [create some campaigns](/campaigns/#creating-a-campaign).

![Sample Campaigns](/articles/quickstart/quickstart-01.png "Sample Campaigns")

> Note, the number of campaigns is limited by your license

Everything in DailyStory is associated with a campaign. For example, if you have a set of customers that you want to enroll in a drip campaign, send emails for a new trial, or track signups on a form, you'll first need a campaign.

And creating a campaign is easy.

We recommend you create campaigns for any marketing activity you want to track or measure. Such as a newsletter campaign, contact us campaign, or adwords campaign.

> When you create any new assets, such as an [Email](/emails/), [Tracking Link](/link-tracking/), or [Landing Page](/pages/) you'll be prompted to either select a campaign or quickly create a new one.

<ol class="step"><li value="3">Create a Lead in your Campaign</li></ol>

Leads are created in your campaigns in several ways:
	
* **Manually** using the + Add Lead button and completing the Create Lead form.
* **Contact Import** [bulk importing new contacts](/contacts/import) and assigning the imported contacts to a campaign.
* **Forms** when visitors complete either a [Web From](/acquisition/web-forms/) or [Magic Form](/acquisition/magic-forms/).
* **Popups** when visitors share their email address in a [popup](/acquisition/popups/).
* **API** when the API is used to create a new lead, such as through [Zapier integration](/integrations/zapier/).

> There is a [contact](/contacts/) for every lead. A contact who is in a campaign is called a lead.

For example, if you have a Newsletter Signups campaign and Elon Musk signs up for your newsletter you will see a new lead in your Newsletter Signups campaign.

![Sample Lead](/articles/quickstart/quickstart-02.png "Sample Lead")

