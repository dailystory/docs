{
title: 'DailyStory Autopilot',
description: 'Automate through Triggers, Actions and Conditions to build user journeys.'
}
#DailyStory Autopilot
Autopilot is DailyStory’s friendly, drag-and-drop automation builder. Using Triggers, Actions and Conditions you can model out complex user journeys and experiences. We put together this guide to help you understand how to use Autopilot.

* **[Triggers](#triggers)**
* **[Actions](#actions)**
* **[Conditions](#conditions)**

## Triggers <a name="triggers"></a>
Triggers are Autopilot blocks that start a workflow. For example, when a form is completed.

**When added to campaign**
The *When added to campaign* trigger adds a lead to the automation workflow when they are added to the campaign. This includes when leads are added through segments, manually, through the API, or through acquisition sources, e.g. Popups.

**When email is opened**
The *When email is opened* trigger adds a lead to the automation workflow when they open a specified email used in the campaign.

**When email is clicked**
The *When email is clicked* trigger adds a lead to the automation workflow when they click a link in a specified email used in the campaign.

**When page is visited**
The *When page is visited* trigger adds a lead to the automation workflow when a specific page is visited. Note, the page must have the DailyStory tracking tag installed.

**When replied to text message**
The *When replied to text message* trigger adds a lead to the automation workflow when reply is received to a text message used in the campaign.

**When popup is submitted**
The *When popup is submitted* trigger adds a lead to the automation workflow when a form is submitted from a [popup](/acquisition/popups/).

**When web form is submitted**
The *When web form is submitted* trigger adds a lead to the automation workflow when a form is submitted from a [web form](/acquisition/web-forms/).

**When magic form is submitted**
The *When magic form is submitted* trigger adds a lead to the automation workflow when a form is submitted from a [magic form](/acquisition/magic-forms/).

**When today's date is**
The *When today's date is* trigger adds a lead to the automation workflow when today's date condition matches the lead's date. For example, [when it is the contact's birthdate](https://www.dailystory.com/blog/send-a-happy-birthday-message/).

**When past date/time**
The *When past date/time* trigger is a special trigger that is used within a workflow. It cannot be the first trigger in the workflow. Instead it is used to to pause the workflow until a specific date/time.

**When time has passed**
The *When time has passed* trigger is a special trigger that is used within a workflow. It cannot be the first trigger in the workflow. Instead it is used to to pause the workflow for a specified number of hours, days, etc.

## Actions <a name="actions"></a>
Actions are Autopilot blocks that do something. For example, send an email.

**Send an email**
The *Send an email* action sends the lead an email if the lead is opted in to receive emails.

**Send a text message**
The *Send a text message* action sends the lead a text message if the lead is opted in to receive text messages and if the lead has a mobile number.

**Send a push notification**
The *Send a push notification* action sends the lead a push notification if the lead is enabled for push notifications.

**Add to segment**
The *Add to segment* action adds the lead/contact to a segment if they do not belong to the segment.

**Remove from segment**
The *Remove from segment* action remove the lead/contact from a segment if they belong to the segment.

**Send an email notification**
The *Send an email notification* action enables you to send an email notification to a user in DailyStory. The notification will automatically include the lead details. A custom message can also be included.

**Send a text message notification**
The *Send a text message notification* action enables you to send a text message notification to a user in DailyStory. The message support personalization tags used to describe the lead, e.g. "{{user.firstname}} visited a page..."

**Change lead status**
The *Change lead status* action changes the status of a lead. A lead's status can be changed from Active to Qualified, Nurturing or another status.

**Add to campaign**
The *Add to campaign* action adds the lead to another campaign (but also leaves the lead in the current campaign). For example, if a lead completes a campaign at the end of the campaign they can automatically be moved to another campaign, such as a nurturing campaign.

**Remove from campaign**
The *Remove from campaign* action removes the current lead from the campaign. For example, if the lead is changed to a nurturing state they may no longer be relevant to the campaign. At DailyStory when a lead converts to a customer we use this action to automatically remove them from the trial campaign. 

**Resend an email**
The *Resend an email* action enables an email that was previously sent to a lead to be resent but with a different subject line. This action is unique because DailyStory does not ordinarily allow a recipient to receive the same email twice. When this action is used the email is able to be sent again to the same recipient. However, the subject line must be different. This ensures that the email does not appear to be a duplicate in the recipient's inbox. [Read more](https://www.dailystory.com/blog/resend-but-with-new-subject-line/)

**Auto-route to subaccount**
The *Auto-route to subaccount* action automatically routes a lead to the subaccount geographically closest to the lead's location. This action is used primarily with DailyStory customers that have various physical locations, such as a fitness franchise with multiple locations. When the lead is routed to the subaccount, DailyStory will create the lead in the subaccount in a campaign named identical to the parent's campaign. If none is found, a new campaign is automatically created and the lead is added.

**Assign points**
The *Assign points* action is used to add or remove points to a lead. For example, if your target market is English speaking countries you could add points for some countries and event remove points for other countries. Points are useful for scoring a lead. Once a lead accumulates a certain point threshold, the lead could become sales qualified, moved to another campaign, tagged or just about anything else you want to do.

**Restart workflow**
The *Restart workflow* action resets a lead within the workflow so that the lead can be processed through the workflow again. For example, an automation that scores a lead for visiting a specific page in your website. The same lead can visit multiple times and this would enable the lead to accumulate additional points on each visit.

## Conditions <a name="conditions"></a>
Conditions are Autopilot blocks that evaluated something. For example, was an email opened. Conditions are unique because they support logic Yes/No branching, i.e. if the email is opened (Yes) or not opened (No).

**Yes**
The *Yes* condition can only be used for branching on the success of another condition.

**No**
The *No* condition can only be used for branching on the failture of another condition.

**Was email opened?**
The *Was email opened?* condition evaluates if an email is opened within a given time window, e.g. 3 hours. If a Yes/No block is not specified, the condition will allow the workflow to continue only if the email is opened.

**Was email clicked?**
The *Was email clicked?* condition evaluates if a link in an email is clicked within a given time window, e.g. 3 hours. If a Yes/No block is not specified, the condition will allow the workflow to continue only if a link in the email is clicked.

**Was text message replied to?**
The *Was text message replied to?* condition evaluates if a reply is received to a text message within a given time window, e.g. 3 hours. If a Yes/No block is not specified, the condition will allow the workflow to continue only if a reply is received.

**Evaluate custom rule**
The *Evaluate custom rule* condition evaluates a series of conditions attempting to match any or all. Using *Evaluate custom rule* Autopilot can evaluate any field, including custom fields. If a Yes/No block is not specified, the condition will allow the workflow to continue only if the rule evaluates successfully.

**Evaluate text message reply**
The *Evaluate text message reply* condition evaluates a reply to a text message. The evaluation is not case sensitive. For example, if the text message reply is "yes" the condition will succeed. If a Yes/No block is not specified, the condition will allow the workflow to continue only if the replied text matches.