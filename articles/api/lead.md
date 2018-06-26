{
	title: 'DailyStory Lead REST API',
	description: 'Documentation for DailyStory\'s  Lead REST API'
}
# Lead REST API
Use the Lead REST API to create or find leads in DailyStory.

> Impor

## Create a Lead or find an existing Lead
To create a lead or find an existing lead you must have an email address and the `Id` of the campaign the lead is part of. You can optionally send additional data as part of the API call.

> If a lead already exists within the campaign, a new lead will not be created and the return value will be the id of the existing lead.

If a lead does not already exist within the campaign, DailyStory will create a new contact and then create a lead in the specified campaign.

<ol class="step"><li value="POST">`/API/Lead`</li></ol>

### Sample request body
The body of the POST must include a JSON representation of the Lead. For example, to create a new lead in campaign 649 with the email api@example.com:
	
<pre class="brush: javascript">
{
	"campaignId": 649,
	"email": "api@example.com"
}
</pre>

To see all the available fields, [login to DailyStory](https://app.dailystory.com/login), and navigate to an existing lead. For example, `Lead/Detail/117604`. Then change the URL to `API/Lead/117604` to see the JSON representation.

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

### Request body fields
<table class="table">
	<thead>
	<tr>
		<th>Field<th>
		<th>Description<th>
		<th>Format<th>
		<th>Required<th>
		</tr>
	</thead>
	<tbody>
	<tr>
	<td>email</td>
	<td>The email address of the lead.</td>
	<td>string</td>
	<td>Yes</td>
	</tr>
	<tr>
	<td>campaignId</td>
	<td>The Id of the campaign the lead is part of.</td>
	<td>number</td>
	<td>Yes</td>
	</tr>
	<tr>
	<td>leadSource</td>
	<td>Where the lead was created</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>description</td>
	<td>Text describing the lead, e.g. the contents from a form.</td>
	<td>string</td>
	<td>No</td>
	</tr>
	</tbody>
</table>

When creating a lead the following fields can also be specified.

> Important - if you are updating an existing lead, these fields will be ignored. Instead you will need to use the Contact API to update fields for an existing Contact.

<table class="table">
	<thead>
	<tr>
		<th>Field<th>
		<th>Description<th>
		<th>Format<th>
		<th>Required<th>
		</tr>
	</thead>
	<tbody>
	<tr>
	<td>salutation</td>
	<td>Mr., Mrs., etc.</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>firstName</td>
	<td>The first name of the person.</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>lastName</td>
	<td>The last name of the person.</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>title</td>
	<td>The person's title</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>numberOfEmployees</td>
	<td>The number of employees or people in the organization</td>
	<td>number</td>
	<td>No</td>
	</tr>
	<tr>
	<td>numberOfEmployees</td>
	<td>The number of employees or people in the organization</td>
	<td>number</td>
	<td>No</td>
	</tr>
	<tr>
	<td>industry</td>
	<td>The <a target="_new" href="https://www.naics.com/search/">Standard Industrial Classification number</a> for the organization</td>
	<td>number</td>
	<td>No</td>
	</tr>
	<tr>
	<td>annualRevenue</td>
	<td>The annual revenue for the organization</td>
	<td>number</td>
	<td>No</td>
	</tr>
	<tr>
	<td>website</td>
	<td>A url for the person or organization</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>address</td>
	<td>A street address</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>country</td>
	<td>The two character country code of the person's location</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>region</td>
	<td>The region or state of the person's location</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>city</td>
	<td>The city of the person's location</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>postalCode</td>
	<td>The postal or zip code of the person's location</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>geoCode</td>
	<td>The latitude and longitude of the person's location</td>
	<td>string, e.g. 47.60621,-122.33207</td>
	<td>No</td>
	</tr>
	</tr>
	<tr>
	<td>company</td>
	<td>The company or organization the person is part of</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>mobilePhone</td>
	<td>Primary or mobile phone, used for Text Message campaigns</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>phone</td>
	<td>Secondary or non-mobile phone</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>avatarPath</td>
	<td>Url to the person's avatar or image</td>
	<td>string</td>
	<td>No</td>
	</tr>
	<tr>
	<td>gender</td>
	<td>Person's gender</td>
	<td>number</td>
	<td>No</td>
	</tr>
	<tr>
	<td>dateOfBirth</td>
	<td>Person's date of birth</td>
	<td>date or null</td>
	<td>No</td>
	</tr>
	</tbody>
</table>


To specify additional data, such as custom fields, use either `extendedProperties` or `leadExtendedProperties`. For example, if a customer downloaded your mobile app from the Apple App Store.

<pre class="brush: javascript">
{
	"leadId": 117604,
	"campaignId": 649,
	...
	"leadExtendedProperties": {
		"appStore": "Apple",
		"downloaded": "2018-07-26T00:18:02.623"
	}
}
</pre>

Custom data added to `leadExtendedProperties` is available within the campaign for personalization, rules, and automations. Custom data added to `extendedProperties` is part of the Contact and can be additionally used for segmentation.

## Sample response body