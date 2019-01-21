{
	title: 'Visit Alerts',
	description: 'Send notification or emails when leads visit pages on your website.'
}
# Visit Alerts
Visit Alerts notify you, or take other actions, when leads in this campaign visit specific pages on your website.

For example, use a Visit Alert to send an email to your sales team when a lead in a campaign visits a page in your website such as a licensing or pricing page. Or, use a Visit Alert to send an email to the visitor immediately or soon after their visit. 

In both examples, a Visit Alert gives you the ability to follow up with a potential customer when they are active and on your website.

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FaAO0iCL7JmM%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DaAO0iCL7JmM&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FaAO0iCL7JmM%2Fhqdefault.jpg&key=internal&type=text%2Fhtml&schema=youtube" width="500" height="281" scrolling="no" frameborder="0" allowfullscreen></iframe>

> To use Visit Alerts, the [DailyStory tracking code](/install) must be included on the page you are monitoring.

**Create and Edit a Visit Alert**

* [Create a Visit Alert](#create-a-visit-alert)
* [Edit a Visit Alert](#edit-a-visit-alert)
* [Setting Visit Alert actions](#visit-alert-actions)

**Frequently Asked Questions**

* [Can I create a Visit Alert for any contact in DailyStory?](#can-i-create-a-visit-alert-for-any-contact-in-dailystory)
* [Why am I receiving an error that the Visit Alert can't be created?](#why-am-i-receiving-an-error-that-the-visit-alert-cant-be-created)
* [How do Visit Alerts work?](#how-do-visit-alerts-work)

## Create a Visit Alert
To create a Visit Alert: 

* Navigate to Acquisition > Visit Alerts and click `+ Create` in the Visit Alerts menu.

![Create Visit Alert](/articles/acquisition/triggers/visitalerts-01.png "Create Visit Alert")

Enter a friendly name for your Visit Alert and the URL for DailyStory to monitor.

* **Name** - friendly name used within DailyStory for the Visit Alert.
* **URL** - full URL that DailyStory will monitor for visits from known leads or customers.

> To use Visit Alerts, the [DailyStory tracking code](/install) must be included on the page you are monitoring.

### Configure Visit Alert actions
Next, configure what happens when a lead visits your URL.

![Visit Alert Actions](/articles/acquisition/triggers/visitalerts-02.gif "Visit Alert Actions")

Actions can be taken on every visit or on a specific visit, such as the 3rd visit. Next, set what action should be taken:

* Send a notification to a user in DailyStory, such as a sales rep.
* Send the visitor (the lead) and email

## Edit a Visit Alert
Edit a Visit Alert by clicking on it from the list of Visit Alerts at Acquisition > Visit Alerts.
	
![All Visit Alerts](/articles/acquisition/triggers/visitalerts-03.png "All Visit Alerts")

Clicking either will open the Visit Alert editor. The same editor used to [Create a Visit Alert](#create-a-visit-alert)

## Visit Alert Actions
A Visit Alert may contain one or more Visit Alert actions. Visit Alert actions are set from the Add Visit Alerts actions popup:

![Visit Alerts actions popup](/articles/acquisition/triggers/visitalerts-04.png "Visit Alerts actions popup")

> If no Visit Alert actions are provided, the Visit Alert is still saved, but does not run.

**When should this alert run** an action can be taken on each visit or on visit 1 - 10. For example, run the Visit Alert the 2nd time a lead visits your page.

**What action should be taken** the action identifies what is done when a lead visits. Either an email notification is sent to a user in DailyStory or an email is sent to the lead that visited the page. The email sent to the lead can be sent immediately, after 15 minutes, after 30 minutes, after 1 hour or after 2 hours.

**Send the notification to** or **Select an email** this option is determined by the action. If the action is to send a notification, the drop down will show a list of DailyStory users that can receive the notification. If the action is the send the lead an email, the drop down is a list of the emails that can be sent to the lead.

## Frequently Asked Questions
Below are some frequently asked questions about Visit Alerts.

### Can I create a Visit Alert for any contact in DailyStory?
Yes, but this is not recommended. Visit Alerts are scoped by campaign. For example, if you have a campaign for a free trial a Visit Alert could be used to see which leads in that campaign visit your licensing and pricing page. Visit Alert activity is associated with the Lead in the campaign too.

### Why am I receiving an error that the Visit Alert can't be created?
First, check to make sure the URL is valid. Next, make sure the DailyStory Trackkng Tag is installed on the page (it is required). If the URL is valid and DailyStory is properly installed, you will see a preview of your page in the editor. If you are still experiencing problems, please [contact us](https://www.dailystory.com/contact-us).

### How do Visit Alerts work?
DailyStory tracks page visits through the [DailyStory tracking code](/install). DailyStory analyzes your page visits and if an identified visitor is found, your Visit Alert is run.

