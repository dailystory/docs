{
	title: 'DailyStory + Mailgun',
	description: 'Integration for DailyStory and Mailgun'
}
# DailyStory + Mailgun
The DailyStory + Mailgun integration enables you to use the power of DailyStory's marketing and automation tools with a powerful transactional email platform: [Mailgun](https://www.mailgun.com/).

DailyStory sends email for you, but with Mailgun integration you can further control how email is sent and ensure that it is authorized to your domain - all to help deliver your email to your customers.
	
> DailyStory takes care of communicating with Mailgun to track delivery and bounces. Open and click tracking is managed by DailyStory.

## Configuring Mailgun Integration
There are several steps required to configure DailyStory and Mailgun integration. These steps are detailed below.

<ol class="step"><li value="1">Create a Mailgun Account</li></ol>
Visit [Mailgun](https://www.mailgun.com) and create an account. There are a few technical steps that will require someone from your IT team to help with.

> If you don't have an IT person or team, we can help.

The good news, it's [free to send up to 10,000 emails](https://www.mailgun.com/pricing-1) per-month!

<ol class="step"><li value="2">Mailgun API Keys</li></ol>
After creating your account and setting everything up, you are ready to connect Mailgun to DailyStory.

Login to Mailgun and visit your Account > Security page. Copy your Private API Key. 

> You do not need the Public Validation Key.

![DailyStory + Mailgun API Keys](/articles/integrations/mailgun-01.png "DailyStory + Mailgun API Keys")

Next, configure DailyStory to use the API keys for your Mailgun account.

<ol class="step"><li value="3">Configure DailyStory</li></ol>
Log into your DailyStory account and navigate to Admin > Integrations and select the Mailgun integration:

![DailyStory + Mailgun](/articles/integrations/mailgun-02.png "DailyStory + Mailgun")

Enter the domain you configured as part of your Mailgun setup, such as <code>mg.example.com</code>.

Next, enter the API Key and click Save.

DailyStory will attempt to send a test email to [the email address you configured for DailyStory](/account/personal-settings) to verify the integration is properly setup.

## Frequently Asked Questions
Below are some frequently asked questions.

### Do I have to setup Mailgun integration to send email?
No, you can send email without configuring Mailgun. However, emails will be send on your behalf and may get flagged as SPAM.

### Do you support SendGrid, Mandrill or other transactional email platforms?
No, currently we only support Mailgun. We plan to offer support for SendGrid in the future.

## Troubleshooting
If you received an error when saving your Mailgun credentials it means that something is misconfigured with Mailgun, your domain or API Key, or there is a problem with your email address.

First, we recommend double-checking the domain and API Key to ensure that the values are the same as the values configured in Mailgun. This is the most common problem.

Next, double-check that the email used by DailyStory is a valid and working email address. The email address can be found in [Admin > Personal Settings](/account/personal-settings). 