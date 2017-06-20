---
layout: _ArticleLayout
title: Salesforce Integration
description: Integration for DailyStory and Salesforce
---
# Salesforce Integration for DailyStory
DailyStory supports integration with Salesforce that enables:
	
* Leads in DailyStory that are marked as Marketing Qualified are automatically pushed as a new lead in Salesforce
* Automatically or manually associate opportunities in Salesforce, such as for new customers or retention, to campaigns in DailyStory.

> DailyStory does not currently enable bi-directional sync with Salesforce. DailyStory can publish leads to Salesforce and read opportunity details.

## Configuring Salesforce Integration
There are several steps required to configure DailyStory and Salesforce integration. These steps are detailed below.

<ol class="step"><li value="1">Create a Salesforce App</li></ol>
Log in to your Salesforce account with administrative rights and go to the Salesforce Setup screen.

On the left menu, select Build > Create > Apps: 
	
![Apps Menu](/articles/integrations/salesforce-01.png "Salesforce Apps")

Next, click New on the Connected App menu:
	
<ol class="step"><li value="2">Configure Salesforce App</li></ol>	
Complete the form for the Connected App:
	
### Basic Information
Enter the name <code>DailyStory Connected App</code> as the name of your application. 

> The API Name should be automatically set. If not, enter <code>DailyStory_Connected_App</code> as the API name. 

Finally, set the contact email to your email address.

![Basic Information](/articles/integrations/salesforce-03.png "Basic Information")

## API
Check <code>Enable OAuth Settings</code>, this will expand the list of available settings.

Set the <code>Callback URL</code> to the value below:

<code>https://app.dailystory.com/API/Public/OAuthCallback/76db0921-55f1-4283-8017-7bd6b6abcbed</code>

Next add all of the <code>Available OAuth Scope</code> to the <code>Selected OAuth Scopes</code>. This ensures that DailyStory has the ability to create leads and read other data from Salesforce.

Next, check <code>Include ID Token</code> and check <code>Include Standard Claims</code>, <code>Include Custom Attributes</code>, and <code>Include Custom Permissions</code>.

![API Information](/articles/integrations/salesforce-04.png "API Information")

Click the Save button. It can take 2-10 minutes for your application to get setup in Salesforce.

<ol class="step"><li value="3">Configure DailyStory</li></ol>	

After saving your new Salesforce app, you should have a view similar to this:
	
![Salesforce App](/articles/integrations/salesforce-05.png "Salesforce App")

Click the <code>Click to reveal</code> link on the <code>Consumer Secret</code>.

Login to DailyStory and go to Integrations.

> To get to Integrations click on the shortcut menu in the top right and click Account Settings. Next, navigate to Integrations using the menu on the left.

Click on Salesforce:
	
![Salesforce Integration](/articles/integrations/salesforce-06.png "Salesforce Integration")

From your DailyStory Connected App in Salesforce copy the values for <code>Consumer Key</code> and <code>Consumer Secret</code> into DailyStory and click Authorize:
	
![Salesforce Integration](/articles/integrations/salesforce-07.png "Salesforce Integration")
