{
title: 'Push Notifications',
description: 'DailyStory Push Notifications'
}
# Push Notifications
DailyStory Push Notifications enable you to create personalized and targeted messages sent to DailyStory [Contacts](/contacts) as part of a [Campaign](/campaigns).

Push Notifications are a powerful tool. Use them to send personalized communication to people using your App. This can include:

* Thank you messages
* Reminders
* Imporant notices
* Offers and discounts

DailyStory's Push Notifications also support personalization and are sent individually to each contact. This is different from other broadcast Push Notification services which send the same message to all recipients.

> Push Notifications will only be sent to Contacts that opted in to receive Push Notifications on their iOS or Android device. Push Notification messages are only available to iOS and Android App(s). And, your iOS or Android App must also [registers the device id](/api/contact/#api-contact-registerdevice) with DailyStory.

DailyStory Push Notifications are sent using [Twilio](/integrations/twilio). [Twilio Notify Service integration](/integrations/twilio) must be configured. DailyStory can manage and configure this service for you, or you can do it yourself.

This guide provides a list of resources to help you get started with Push Notifications.

**Create and Edit a Push Notification**

* [Create a Push Notification](#create-a-push-notification)
* [Edit a Push Notification](#edit-a-push-notification)
* [Send a Test Push Notification](#test-a-push-notification)

**Frequently Asked Questions**

* [Is everyone sent the same Push Notification?]
* [Can I personalize the content in the Push Notification?]
* [Why didn't my contact receive a Push Notification?]
* [Can one contact have multiple devices?]
* [How do I enable DailyStory to send Push Notification to my App?]
* [Why do I see Preview Unavailable?]
* [Why can't I see delivery information?]

## Create a Push Notification
To create a new Push Notification, navigate to Content > Push Notifications. Next, in the main Push Navigation menu click `+ Create`. This will open the Push Notification editor.

When the editor opens select the campaign this Push Notification is used within or create a new campaign.

Next, select a title and content for the Push Notification. As you type your title and content you'll see a preview of what your Push Notification will look like.

![Create Push Notification](/articles/push-notifications/push-03.gif "Create Push Notification")

> Recommended title and message length vary between devices. However, in general, a Push Notification should be as short as possible.

Finally, Save the Push Notification. 

Once the Push Notification is saved you can also [schedule when](#send-a-push-notification) and to whom the Push Notification is sent to. The Push Notification is also now available to add to a campaign's workflow.

## Edit a Push Notification
To edit a Push Notification navigate to Content > Push Notifications and click the Push Notification you want to edit.

![All Push Notifications](/articles/push-notifications/push-04.png "All Push Notifications")

This will open the Edit Push Notification screen. This screen is nearly identical to the Create Push Notification screen.

> If you edit the content of a scheduled Push Notification, the scheduled Push Notification will use your new content.

## Test a Push Notification
There are two options for sending a test Push Notification.

### 1. Send a test from the Push Notification editor
Clicking the `Send Test` button in the Push Notification editor will open a popup. Search for and select a Contact that you wish to send the Push Notification to.

> Sending a test Push Notification will only send the Push Notification message to the specified contact.

![Send Test Push Notification](/articles/push-notifications/push-05.png "Send Test Push Notification")

If the Contact has a device registered for Push Notifications and has not opted out, the test message will be sent to the Contact's devices.

### 2. Use Push Notification tools to send a test Push Notification
DailyStory includes several tools for testing Push Notifcations. If you have access to the Administration section, navigate to Account Settings > Tools and find the Push Notifications section.

![Push Notification Tools](/articles/push-notifications/push-02.png "Push Notification Tools")

Using these advanced tools you can verify if a Contact has a registered Device Binding, manually register a Device Binding for a Contact, or Send a Push notification to a specific Contact. 

> Sending a test Push Notification will only send the Push Notification message to the specified contact.

## Send a Push Notification
Similar to other features such as [Email](/emails) and [Text Messages](/text-messages), Push Notifications are sent through [Campaign Workflows](/campaigns/workflows) and [Campaign Schedules](/campaigns/schedules).

### Send using Scheduler
To send a Push Notification using a Campaign's Schedule edit the Push Notification and scroll down and set the segments to send to and the date and time to send.

For example, to send to customers in the 'Upcoming appointments' segment at 10am.

> Send dates and times are based on the [Timezone](/account/settings) configured for your account.

### Send using Workflow
To send a Push Notification using a Campaign's Workflow. Add a Push Notification Workflow Step and select the Push Notification to send.

![Push Notification](/articles/push-notifications/push-01.png "Push Notification")

## Frequently Asked Questions
Below are frequently asked questions about Push Notifications:

### Is everyone sent the same Push Notification?
### Can I personalize the content in the Push Notification?
### Why didn't my contact receive a Push Notification?
### Can one contact have multiple devices?
### How do I enable DailyStory to send Push Notification to my App?
### Why do I see Preview Unavailable?
### Why can't I see delivery information?
### What is a Device Binding?
