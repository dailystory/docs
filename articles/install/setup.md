{
	title: 'Technical Setup Guide',
	description: 'Instructions for configuring DailyStory'
}
# Technical Setup Guide
This setup guide, designed for configuring advanced options for your use of DailyStory, requires some IT or technical knowledge. If this doesn't describe you, just [drop us a note](mailto:hello@dailystory.com) and we can help.

## Add a custom subdomain
Setting up a subdomain enables content hosted by DailyStory, such as your landing page, to appear as part of your domain.

* [Instructions for configuring a custom subdomain](/install/subdomain)

### Optionally configure Email and a Domain
You can start using DailyStory without setting up email or a custom domain. Email will be sent on your behalf through DailyStory's email system and your pages and content will be hosted on DailyStory's domain.

People that receive your email will see the message as coming from:
	
`Anna Jones <anna@example.com> on behlaf of DailyStory`

Landing pages or other content hosted on DailyStory will look like:
	
`https://dlystr.io/Sample-landing-page?_UID=4933ca402181fcf4a5c94713daaa9921`

To configure your own email account and subdomain, please [follow the steps in our technical setup guide](/install/setup)

## Frequently Asked Questions
Below are some frequently asked questions.

### Where can I find my tenant ID?
Each tenant in DailyStory is run in a geographical instance and is assigned a unique tenant ID. The tenant ID is used within the application, in the JavaScript API, and in the REST API. If you need to find the ID of your tenant you can do so in several ways:
	
#### Use the JavaScript API
Open a console window in your browser and type:

`Ds.id`

You should see a unique identifier as the output.

![DailyStory Tenant Id](/articles/setup/setup-01.png "DailyStory Tenant Id")

#### From your Tenant
When logged into your tenant, go to `/admin/about`. This will show your instance id, data center id, and unique tenant id.

![DailyStory Tenant Id](/articles/setup/setup-02.png "DailyStory Tenant Id")

