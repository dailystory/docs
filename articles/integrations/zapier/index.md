{
	title: 'Zapier integration',
	description: 'Integration for DailyStory and Zapier'
}
# Zapier Integration for DailyStory
DailyStory's [Zapier integration](https://zapier.com) enables you to connect DailyStory with thousands of other applications using Zapier’s Triggers and Actions:

* A Zapier Trigger listens for events that occur in your applications. For example, you can create a Zapier Trigger for Gmail that looks for certain emails.

* A Zapier Action defines an action to be taken in your applications. For example, creating a new lead in DailyStory.

> A Trigger combined with one or more Actions is called a “Zap”.

DailyStory’s Zapier support includes both Triggers and Actions specific to DailyStory.

## Configuring Zapier Integration
There are several steps required to configure DailyStory and Zapier integration. These steps are detailed below.

<ol class="step"><li value="1">Create a Mailgun Account</li></ol>
Visit [Zapier](https://www.zapier.com) and create an account.

<ol class="step"><li value="2">Create a DailyStory API key</li></ol>
Visit [Zapier](https://www.zapier.com) and create an account.

## DailyStory Triggers
DailyStory provides several Zapier Triggers:

![DailyStory Zapier Triggers](/articles/integrations/zapier/zapier-02.png "DailyStory Zapier Triggers")

* Link Click - if a DailyStory [tracking link](/link-tracking/) is clicked.
* New Lead - if a new [Lead](/leads/) in DailyStory is created.
* Page Visit - if a page configued for [lead visit alerts](/acquisition/triggers/) is visited.

## DailyStory Actions
DailyStory provides several Zapier Actions:

![DailyStory Zapier Actions](/articles/integrations/zapier/zapier-01.png "DailyStory Zapier Actions")

* Create or Update Lead - called first after any trigger to ensure that a lead is created in the correct campaign. It returns the ID of the lead. This id can be used with the Add Lead Activity action as well.
* Create or Update Contact - creates or updates a contact in DailyStory, but does not add the contact to a campaign.
* Add Lead Activity - easily add details to the lead about the type of activity the lead participated in, for example [Attended GoToWebinar meeting](/integrations/zapier/gotowebinar).
* Send Email - sends an email to a given lead.

## Common Use Cases
* [GoToWebinar](/integrations/zapier/gotowebinar#capture-gotowebinar-attendees)


