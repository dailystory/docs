{
	title: 'Technical Setup Guide',
	description: 'Instructions for configuring DailyStory'
}
# Technical Setup Guide
This setup guide is designed for IT or technical people. If this doesn't describe you, just [drop us a note](mailto:hello@dailystory.com).

## Custom subdomain
Setting up a subdomain to point to DailyStory enables content hosted by DailyStory, such as your landing page, to appear as part of your domain.

For example, without a subdomain pages hosted by DailyStory will appear as:
	
`https://dlystr.io/Sample-landing-page?_UID=4933ca402181fcf4a5c94713daaa9921`

With a subdomain pages hosted by DailyStory will appear as:

`https://[your domain]/Sample-landing-page`

### Setup a custom subdomain
Below are the steps required to setup a custom subdomain.

<ol class="step"><li value="1">Choose a subdomain</li></ol>
First, choose a subdomain and ensure it isn't already in use. We recommend: pages.[your domain].

<ol class="step"><li value="2">Configure DNS CNAME record</li></ol>
Once you have selected a subomain you will need to create a CNAME DNS entry to point your domain to DailyStory. Configure your CNAME record to resolve to `pages.dailystory.net` with a TTL of at least 3600.

<ol class="step"><li value="3">Verify the DNS change</li></ol>
It can take several hours for a DNS change to propogate. You can check the status of your DNS entry using DNS lookup tools such as [Uptrends](https://www.uptrends.com/tools/dns), [MX Toolbox](https://mxtoolbox.com/), and others.

Using these tools will enable you to see if your new DNS entry is properly resolving to DailyStory.

<ol class="step"><li value="4">Notify Us</li></ol>
DailyStory's software runs in Microsoft's Azure cloud. Because of security, if you test your new domain by going to it in a browser it will resolve to a landing page managed by Microsoft Azure and not to a page managed by DailyStory.

To enable DailyStory to serve content for your domain you need to [send an email to us](hello@dailystory.com)


### Optionally configure Email and a Domain
You can start using DailyStory without setting up email or a custom domain. Email will be sent on your behalf through DailyStory's email system and your pages and content will be hosted on DailyStory's domain.

People that receive your email will see the message as coming from:
	
`Anna Jones <anna@example.com> on behlaf of DailyStory`

Landing pages or other content hosted on DailyStory will look like:
	
`https://dlystr.io/Sample-landing-page?_UID=4933ca402181fcf4a5c94713daaa9921`

To configure your own email account and subdomain, please [follow the steps in our technical setup guide](/install/setup)
