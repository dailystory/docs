{
	title: 'Technical Setup Guide',
	description: 'Instructions for configuring DailyStory'
}
# Technical Setup Guide
This setup guide, designed for configuring advanced options for your use of DailyStory, requires some IT or technical knowledge. If this doesn't describe you, just [drop us a note](mailto:hello@dailystory.com) and we can help.

## Add a custom subdomain
Setting up a subdomain enables content hosted by DailyStory, such as your landing page, to appear as part of your domain.

* [Instructions for configuring a custom subdomain](/install/subdomain)

## Send from your email address
Unless configured, email sent on your behalf by DailyStory will use one of DailyStory's email domains. 

This means that people that receive your email will see the message as coming from:
	
`Anna Jones <anna@example.com> on behalf of DailyStory`

But more importantly, the SPF and DKIM records that verify that the sender is allowed to send on behalf the domain will fail. This can have a significant impact on the deliverbility of your email as some email server will reject or flag your message as SPAM.

We recommend setting up integration with Mailgun.

* [Instructions for setting up Mailgun integration](/integrations/mailgun)

## Frequently Asked Questions
Below are some frequently asked questions.

### Where can I find my tenant ID?
Each tenant in DailyStory is run in a geographical instance and is assigned a unique tenant ID. The tenant ID is used within the application, in the JavaScript API, and in the REST API. If you need to find the ID of your tenant you can do so in several ways:
	
#### Use the JavaScript API
Open a console window in your browser and type:

`Ds.id`

You should see a unique identifier as the output.

![DailyStory Tenant Id](/articles/install/setup-01.png "DailyStory Tenant Id")

#### From your Tenant
When logged into your tenant, go to `/admin/about`. This will show your instance id, data center id, and unique tenant id.

![DailyStory Tenant Id](/articles/install/setup-02.png "DailyStory Tenant Id")

