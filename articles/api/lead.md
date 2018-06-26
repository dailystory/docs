{
	title: 'DailyStory Lead REST API',
	description: 'Documentation for DailyStory\'s  Lead REST API'
}
# Lead REST API
Use the Lead REST API to create or find leads in DailyStory.

> Impor

## Create a Lead
To create a lead you must have an email address and the `Id` of the campaign the lead is part of. You can optionally send additional data as part of the API call.

> If a lead already exists within the campaign, a new lead will not be created and the return value will be the id of the existing lead.

> If a lead does not already exist within the campaign, DailyStory will create a new contact and then create a lead in the specified campaign.

<ol class="step"><li value="POST">`/API/Lead`</li></ol>

### Sample request body
The body of the POST must include a JSON representation of the Lead. For example, to create a new lead in campaign 649 with the email api@example.com:
	
<pre class="brush: javascript">
{
	"campaignId": 649,
	"email": "api@example.com"
}
</pre>

To see all the available fields, [login to DailyStory](https://app.dailystory.com/login), and navigate to an existing lead. For example, `Lead/Detail/117604`, and change the URL to `API/Lead/117604` to see the JSON representation of this lead.

<pre class="brush: javascript">
{
	"leadId": 117604,
	"campaignId": 649,
	"ip": "",
	"leadSource": "Contact List",
	"points": 0,
	"score": 0.00,
	"workflowStepId": 0,
	"leadStatus": "Active",
	"leadOrigin": "List",
	"leadOriginId": "2",
	"leadOriginName": "Unit Test List",
	"leadExtendedProperties": {},
	"leadUID": "b685dd4acc364ac38cf1e75581ff187b-117604",
	"Description": "",
	"dsId": "b685dd4acc364ac38cf1e75581ff187b",
	"salutation": "",
	"firstName": "",
	"lastName": "",
	"optOut": false,
	"email": "api@example.com",
	"title": "",
	"status": "Active",
	"company": "Trial Account",
	"numberOfEmployees": 0,
	"industry": 0,
	"annualRevenue": 0,
	"website": "",
	"phone": "",
	"mobilePhone": "",
	"timezone": "",
	"avatarPath": "",
	"country": "",
	"city": "",
	"postalCode": "",
	"address": "",
	"geoCode": "",
	"dateFirstSeen": "1753-01-01T00:00:00",
	"dateLastSeen": "1753-01-01T00:00:00",
	"region": "",
	"gender": 0,
	"dateBirth": null,
	"age": 0,
	"extendedProperties": {},
	"dateContactCreated": "2018-03-26T00:00:00",
	"timestampCreated": "2018-03-26T02:45:36.623",
	"dateContactLastModified": "2018-06-26T00:18:02.623",
	"dateLastContacted": "2018-06-26T00:18:02.623",
	"accountId": 0
}
</pre>

To specify additional data, such as custom fields, use either `extendedProperties` or `leadExtendedProperties`. For example, if a customer downloaded your mobile app from the Apple App Store.

<pre class="brush: javascript">
{
	"leadId": 117604,
	"campaignId": 649,
	...
	"leadExtendedProperties": {
		"appStore": "Apple",
		"downloaded": 	"2018-07-26T00:18:02.623"
	}
}
</pre>

Custom data added to `leadExtendedProperties` is available within the campaign for personalization, rules, and automations. Custom data added to `extendedProperties` is part of the Contact and can be used for segmentation.

## Sample response body