{
	title: 'Salesforce Integration',
	description: 'Integration for DailyStory and Salesforce'
}
# Salesforce Integration for DailyStory
DailyStory supports integration with Salesforce that enables:
	
* Leads in DailyStory that are marked as Marketing Qualified are automatically created as a new lead in Salesforce.
* Salesforce Opportunities can be associated with a DailyStory campaign.

> DailyStory does not currently enable bi-directional sync with Salesforce. DailyStory can publish leads to Salesforce and read opportunity details.

## Configuring Salesforce Integration
There are several steps required to configure DailyStory and Salesforce integration. These steps are detailed below.

<ol class="step"><li value="1">Create a Salesforce App</li></ol>
Log in to your Salesforce account with administrative rights and go to the Salesforce Setup screen.

On the left menu, select Build > Create > Apps: 
	
![Apps Menu](/articles/integrations/salesforce-01.png "Salesforce Apps")

Next, click New on the Connected App menu:

![New Connected App](/articles/integrations/salesforce-02.png "New Connected App")
	
<ol class="step"><li value="2">Configure Salesforce App</li></ol>	
Complete the form for the Connected App:
	
### Basic Information
Enter the name <code>DailyStory Connected App</code> as the name of your application. 

> The API Name should be automatically set. If not, enter <code>DailyStory_Connected_App</code> as the API name. 

Finally, set the contact email to your email address.

![Basic Information](/articles/integrations/salesforce-03.png "Basic Information")

Optionally set other fields:
* Logo image URL: https://ds-cdn.azureedge.net/files/brand/125x125.png
* Icon URL: https://ds-cdn.azureedge.net/files/brand/16x16.png
* Info URL: https://docs.dailystory.com/integrations/salesforce
* Description: Used to connect DailyStory and Salesforce


## API
Check <code>Enable OAuth Settings</code>, this will expand the list of available settings (see the screen shot below).

Set the <code>Callback URL</code> to the following value:

https://app.dailystory.com/API/Public/OAuthCallback/76db0921-55f1-4283-8017-7bd6b6abcbed

Next add all of the <code>Available OAuth Scopes</code> to the <code>Selected OAuth Scopes</code>. This ensures that DailyStory has the ability to create leads and read other data from Salesforce.

> These authorization scopes ensure DailyStory has enough permission to perform existing actions as well as for planned integrations.

Next, check <code>Include ID Token</code> and check <code>Include Standard Claims</code>, <code>Include Custom Attributes</code>, and <code>Include Custom Permissions</code>.

![API Information](/articles/integrations/salesforce-04.png "API Information")

Click the Save button. It can take 2-10 minutes for your application to get setup in Salesforce.

After saving your new Salesforce app, you should have a view similar to this:

![Salesforce App](/articles/integrations/salesforce-05.png "Salesforce App")

<ol class="step"><li value="3">Configure DailyStory</li></ol>	

Login to DailyStory and go to Integrations.

> To get to Integrations click on the shortcut menu in the top right and click Account Settings. Next, navigate to Integrations using the menu on the left.

Click on Salesforce:
	
![Salesforce Integration](/articles/integrations/salesforce-06.png "Salesforce Integration")

From your DailyStory Connected App in Salesforce copy the values for <code>Consumer Key</code> and <code>Consumer Secret</code> into DailyStory and click Authorize.

> You may be requested to sign in to Salesforce again

## Advanced Configuration
Once Salesforce integration is enabled you will also be able to configure several advanced Salesforce integration options.

### Extended Field Mappings
DailyStory will automatically populate common Salesforce fields that correspond to properties of a DailyStory lead, for example email address.

However, if you are using a custom form or setting extended lead properties, you may want to publish these into Salesforce as well. This is precisely what the Advanced Configuration option for Extended Field Mappings does.

For example, if you are capturing a values for <code>CurrentSubscribers</code> and you have a Salesforce custom field called <code>NumberOfSubscribers__c </code> you can configure DailyStory to populate that field in Salesforce when a lead is added from DailyStory.

![Salesforce Extended Field Mappings](/articles/integrations/salesforce-07.png "Salesforce Extended Field Mappings")
 