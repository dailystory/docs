{
title: 'Push Notifications',
description: 'DailyStory Push Notifications'
}
# Push Notifications
DailyStory Push Notifications enable you to create personalized and targeted messages sent to DailyStory [Contacts](/contacts) as part of a [Campaign's Workflow](/campaigns). Push Notification messages are delivered to iOS and Android App(s).

> Push Notifications will only be sent to Contacts that opted in to receive Push Notifications on their iOS or Android device and the App [registers the device id](/api/contact/#api-contact-registerdevice) with DailyStory.

DailyStory Push Notifications are sent using [Twilio](/integrations/twilio) and the Twilio Notify Service integration must be configured.

## Creating a Push Notification
Unlike features such as [Email](/emails), Push Notifications are only configured within a Campaign's Workflow.

To create a new Push Notification, navigate to a Campaign's Workflow and add a "Push Navigation":

![Push Notification](/articles/push-notifications/push-01.png "Push Notification")

Next, set the title and message content.

> Recommended title and message length vary between devices. However, in general, a Push Notification should be as short as possible.

## Testing Push Notifications
DailyStory includes several tools for testing Push Notifcations. If you have access to the Administration section, navigate to /tools and find the Push Notifications section:

![Push Notification Tools](/articles/push-notifications/push-02.png "Push Notification Tools")

Using these advanced tools you can verify if a Contact has a registered Device Binding, manually register a Device Binding for a Contact, or Send a Push notification to a specific Contact. 