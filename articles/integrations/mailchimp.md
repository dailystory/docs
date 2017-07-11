---
layout: _ArticleLayout
title: MailChimp Integration
description: Integration for DailyStory and MailChimp
---
# MailChimp Integration for DailyStory
DailyStory is built to send personalized 1:1 emails. For bulk email marketing, such as a newsletters, we recommend using MailChimp. DailyStory's integration with MailChimp enables you to easily add contacts to MailChimp lists after progressing them through a [DailyStory Workflow](/features/workflow).
 
> DailyStory does not currently enable bi-directional sync with MailChimp. Changes to customer information within MailChimp is not reflected in DailyStory.

## Configuring MailChimp Integration
There are several steps required to configure DailyStory and MailChimp integration. These steps are detailed below.

<ol class="step"><li value="1">Create a MailChimp Account</li></ol>
To get started you will need to create an account on <a target="_blank" rel="noopener noreferrer" href="https://mailchimp.com">MailChimp</a> and <a target="_blank" rel="noopener noreferrer" href="http://kb.mailchimp.com/lists/growth/create-a-new-list">create one or more lists</a>. For example, a newsletter list.

<ol class="step"><li value="2">MailChimp API Keys</li></ol>
Once you have a MailChimp account and one or more lists created, you will need to get your API. Within MailChimp first navigate to your MailChimp Account:

![MailChimp Account](/articles/integrations/mailchimp-01.png "MailChimp Account")

Within Account select Extras > API Keys:

![MailChimp Account API Keys](/articles/integrations/mailchimp-02.png "MailChimp Account API Keys")	

Next, click "Create A Key":

![Create API Key](/articles/integrations/mailchimp-03.png "Create API Key")

This will create a new API key displayed in a textbox (blurred out below):

![Copy API Key](/articles/integrations/mailchimp-04.png "Copy API Key")

Copy this API key as we'll need it next.
	
<ol class="step"><li value="3">Configure DailyStory</li></ol>
Login to DailyStory and go to Integrations.

> To get to Integrations click on the shortcut menu in the top right and click Account Settings. Next, navigate to Integrations using the menu on the left.

Click on MailChimp:

![MailChimp Integration](/articles/integrations/mailchimp-05.png "MailChimp Integration")
	
Enter the API Key from MailChimp and click Save. 

Once MailChimp integration is enabled you can add a 'Add lead to MailChimp List' in a Campaign's Workflow and select the Mailing List to add that contact to:

![Workflow Step](/articles/integrations/mailchimp-06.png "Workflow Step")
