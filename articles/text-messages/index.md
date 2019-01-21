{
title: 'Text Messages',
description: 'DailyStory Text Messages'
}
# Text Messages
Use DailyStory Text Messages to send personalized and targeted messages to your [Contact's](/contacts) mobile device.

Text Messages are a powerful tool. Use them to send personalized communication to your customers mobile devices. This can include:

* Thank you messages
* Reminders
* Imporant notices
* Offers and discounts

DailyStory's Text Messages support personalization and are sent individually to each contact. This is different from other broadcast Text Messaging services which send the same message to all recipients.

> Text Messages are sent to Contacts that opted in to receive Text Messages and have a valid mobile phone number.

DailyStory Text Messages require [Twilio](/integrations/twilio) integration. DailyStory can manage and configure this service for you, or you can do it yourself.

> **important** unless included, use of Text Messaging will incur overage charges in your DailyStory account. These charges are pass-through costs from the phone companies that charge per-SMS part. See [Understanding Text Messaging costs](#understanding-text-messaging-costs) for more detail.

This guide provides a list of resources to help you get started with Text Messages.

**Create and Edit a Text Message**

* [Create a Text Message](#create-a-text-message)
* [Edit a Text Message](#edit-a-text-message)
* [Send a test Text Message](#test-a-text-message)
* [Understanding Text Messaging costs](#understanding-text-messaging-costs)

**Frequently Asked Questions**

* [Is everyone sent the same Text Message?](#is-everyone-sent-the-same-text-message)
* [Can I personalize the content in the Text Message?](#can-i-personalize-the-content-in-the-text-message)
* [Why didn't my contact receive a Text Message?](#why-didnt-my-contact-receive-a-text-message)
* [How do I enable DailyStory to send Text Messages?](#how-do-i-enable-dailystory-to-send-text-messages)
* [Can I use emojis in my Text Messages?](#can-i-use-emojis-in-my-text-messages)
* [What happens if someone replies STOP?](#what-happens-if-someone-replies-stop)
* [Can I choose the number Text Messages originate from?](#can-i-choose-the-number-text-messages-originate-from)

## Create a Text Message
To create a Text Message, navigate to Content > Text Messages. Next, in the main Text Messages menu click `+ Create`. This will open the Text Message editor.

When the editor opens select the campaign this Text Message is used within or create a new campaign.

Next, select a name and message for the Text Message. As you type your content you'll see a preview of what your Text Message will look like. The Name of your Text Message is only used internally within DailyStory.

![Create Text Message](/articles/text-messages/textmessages-01.gif "Create Text Message")

> Recommended message length is 160 characters. Exceeding this length will still deliver this as a single message, but it is then considered multiple SMS messages. Please see [Understanding Text Messaging costs](#understanding-text-messaging-costs).

As you type your message, you will also see helpful information under your message update with the number of characters and segments your message uses.

Finally, Save the Text Message. 

Once the Text Message is saved you can also [schedule when](#send-a-text-message) and to whom the Text Message is sent to. The Text Message is also now available to add to a campaign's workflow.

## Edit a Text Message
To edit a Text Message navigate to Content > Text Messages and select the Text Message to edit.

![All Text Messages](/articles/text-messages/textmessages-02.png "All Text Messages")

This will open the Edit Text Message screen. This screen is nearly identical to the Create Text Message screen.

> If you edit the content of a scheduled Text Message, the scheduled Text Message will use your new content.

## Test a Text Message
Clicking the `Send Test` button in the Text Message editor will open a popup. 

By default, the mobile number in the popup will be set to the mobile number in your [Personal Settings](/account/personal-settings#contact-details).

> Sending a test Text Message will only send the Text Message to the specified mobile number.

![Send Test Text Message](/articles/text-messages/textmessages-03.gif "Send Test Text Message")

## Send Text Messages
Similar to other features such as [Email](/emails) and [Push Notifications](/push), Text Messages are sent through [Campaign Workflows](/campaigns/workflows) and [Campaign Schedules](/campaigns/schedules).

### Send using Scheduler
To send a Text Message using a Campaign's Schedule edit the Text Message and scroll down and set the segments to send to and the date and time to send.

For example, to send to customers in the 'Upcoming appointments' segment at 10am.

![Schedule Text Message](/articles/text-messages/textmessages-04.gif "Schedule Text Message")

> Send dates and times are based on the [Timezone](/account/settings) configured for your account.

### Send using Workflow
To send a Text Message using a Campaign's Workflow. Add a Text Message Workflow Step and select the Text Message to send.

![Workflow Text Message](/articles/text-messages/textmessages-05.png "Workflow Text Message")

> Unlike a send that is scheduled, a workflow applies to everyone in the campaign.

## Understanding Text Messaging costs
DailyStory Text Messages requires [Twilio integration](/integrations/twilio). Twilio provides the infrastructure service for sending Text Messages.

Because telecommunication companies charge per-Text Message, it's important to understand how this cost impacts you.

> DailyStory can manage your Twilio account for you and bill for overages or you can setup your own account and provide that information to DailyStory.

[Twilio's pricing is published here](https://www.twilio.com/pricing). Programmable SMS, the service DailyStory uses to actually send your Text Messages has a cost of $0.0075 per-message.

### Character count and segments
A Text Message may contain up to 160 characters. If the message length exceeds 160 characters, the message is still delivered as a single message to most modern devices. However, the message may be broken into multiple message parts known as a segment.

For example, this message contains 180 characters and is broken into 2 segments. 

![Text Message segments](/articles/text-messages/textmessages-06.png "Text Message segments")

> DailyStory provides some helpful information below the message for the approximate character count and number of segments required to send the message. However, is provided as guidance only.

Because of this, the cost for sending this Text Message is $0.0075 * 2 = **$0.015**/per-message. 

This would then be multiplied by the number of people the message is sent to. For example, if the Text Message is sent to 500 contacts the cost is **$7.50** ($0.015 * 500).

#### Using non-standard characters
While the character count for a Text Message is limited to 160 characters, not all characters are created equal. For example, because emojis use special character sets, a single emjoi may require use of an additional segment to send the message.

#### Handling message replies
If a recipient of a Text Message replies to the Text Message, this too incurs a message cost.

#### Opt out of Text Messages
If a recipient replies to a Text Message with "STOP", they are opted out of future Text Messages from the sending number.

## Frequently Asked Questions
Below are frequently asked questions about Text Messages:

### Is everyone sent the same Text Message?
No. Each Text Message sent by DailyStory is send indivudally to each recipient. This is done so each message can be personalized to each recipient.

### Can I personalize the content in the Text Message?
Yes! Using DailyStory's Personalization tags you can add personalized content to your Text Messages.

### Why didn't my contact receive a Text Message?
There are several reasons why a recipient did not receive your Text Message: 

* The mobile number for the recipient is not capable of receiving Text Messages;
* The recipient may not have been included in the segment the Text Messages was sent to; 
* The recipient may not have opted-in to receive Text Messages;

### How do I enable DailyStory to send Text Messages?
Enabling DailyStory to send Text Messages requires [Twilio integration](/integrations/twilio) is configured. DailyStory can manage and configure this service for you, or you can do it yourself.

### Can I use emojis in my Text Messages?
Yes! You can use emojis in your Text Messages. However, because emojis are not considered standard text, each emoji impacts the size of your Text Message. Please see [Understanding Text Messaging costs](#understanding-text-messaging-costs) for more detail.

### What happens if someone replies STOP?
If a recipient replies with STOP, they are automatically opted out of receiving Text Messages.

### Can I choose the number Text Messages originate from?
Yes, you can provide the area code that Text Messages arrive from. Please let us know which area code you prefer and we can help configure.