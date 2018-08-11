{
	title: 'DailyStory + Twilio',
	description: 'Integration for DailyStory and Twilio'
}
# DailyStory + Twilio
The DailyStory + Twilio integration enables you to use the power of DailyStory's marketing and automation tools with a powerful cloud communications platform: [Twilio](https://www.twilio.com/).

When enabled, Twilio allows you to: 
* Send SMS messages to your Contact's mobile phone number.
* Send Push notifications to iOS and Android apps registered to your Contacts.
	
> DailyStory takes care of communicating with Twilio to track delivery and clicks in SMS messages.

## Configuring Twilio Integration
There are several steps required to configure DailyStory and Twilio integration. These steps are detailed below.

<ol class="step"><li value="1">Create a Twilio Account</li></ol>
Visit [Twilio](https://www.twilio.com) and create an account. You can create a free account that comes with enough credits for you to experiment with DailyStory's Twilio integration.

> Before you can use the Twilio integration you'll need to select a phone number within Twilio.

<ol class="step"><li value="2">Twilio API Credentials</li></ol>
After creating your account and setting everything up, you are ready to connect Twilio to DailyStory.

Login to Twilio and click *Show API Credentials* in the top right. Copy your *Account SID* and *Auth Token*

![DailyStory + Twilio API Credentials](/articles/integrations/twilio-01.png "DailyStory + Twilio API Keys")

<ol class="step"><li value="3">Twilio Phone Number (optional)</li></ol>

To enable DailyStory to send SMS/Text Messages, you need to configure a phone number in Twilio.

> At this time DailyStory only supports a single phone number.

Once you have created a phone number in Twilio, you can find it in your Twilio console:

![Twilio Phone Number](/articles/integrations/twilio-02.png "Twilio Phone Number")

<ol class="step"><li value="4">Twilio Notify (optional)</li></ol>

To enable DailyStory to send push notifications to your app running on your customers' iOS and Android devices, you need to create a service in Twilio Notify.

> Note, there are additional steps required to configure Twilio for Apple Push Notification and Android Notifications.

Once you have created a Notify Service, copy the Service Id (SID).

![Twilio Service Id](/articles/integrations/twilio-03.png "Twilio Service Id")

Next, configure DailyStory to use the credentials, phone number and service id.

<ol class="step"><li value="5">Configure DailyStory</li></ol>
Log into your DailyStory account and navigate to Admin > Integrations and select the Twilio integration:

![DailyStory + Twilio](/articles/integrations/twilio-04.png "DailyStory + Twilio")

Enter the *Account SID*, *Auth Token*, *Phone Number*, *Service Id*.

> The Service Id is optional, but the all other fields are required.

Next, click Save.

DailyStory will attempt to send a test SMS to [the phone number you configured for DailyStory](/account/personal-settings) to verify the integration is properly setup.

## Frequently Asked Questions
Below are some frequently asked questions.

### Do I have to setup Twilio integration to send SMS/Text Messages?
Yes, if you want to send SMS/Text Messages to your customers as part of a campaign you must configure Twilio.

### Do I have to setup a Notify Service to send SMS/Text Messages?
No, only setup a Notify Service (and set a Service Id in DailyStory) if you have an iOS or Android app that you would like DailyStory to integrate with.

### Do you support other communication platforms?
No, currently we only support Twilio. We are considering supporting additional cloud communication platforms in the future.

## Troubleshooting
If you received an error when saving your Twilio credentials it means that something is misconfigured with Twilio. 

First, we recommend double-checking the Account SID and Auth Token to ensure that the values are the same as the values provided in Twilio. This is the most common problem.

Next, double-check that the mobile phone number used by DailyStory is a valid and working. The mobile phone can be found in [Admin > Personal Settings](/account/personal-settings). 
