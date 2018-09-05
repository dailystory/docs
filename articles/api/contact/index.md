{
	title: 'DailyStory Contact REST API',
	description: 'Documentation for DailyStory\'s Contact REST API'
}
# Contact REST API
Use the Contact REST API to create, update or delete Contacts.

## API Contact
The Contact API is used to create or update a single contact `POST`, retrieve a contact `GET`, or delete a contact `DELETE`.

> If a contact already exists, the contact is updated with any new values.

<ol class="api"><li value="GET">/API/Contact/[DSID]</li></ol>

Sending a `GET` request with the DSID of the Contact you wish to retrieve. To see this in action, [login to DailyStory](https://app.dailystory.com/login) and navigate to an existing contact. For example, `/Contact/Detail/1359c31a651f4684a04c6e9d12ec154d`. Then change the URL to `API/Contact/1359c31a651f4684a04c6e9d12ec154d` to see the JSON representation.

### Sample response body
Returns `200 OK` when created. The body of the response includes a JSON object with additional data with the `DSID` of the Contact.

<pre class="brush: javascript">
{
"Status": true,
"Message": "",
"Code": 200,
"Response": {
"contact": {
"dsId": "1359c31a651f4684a04c6e9d12ec154d",
"salutation": "",
"firstName": "Ben",
"lastName": "Smith",
"optOut": false,
"email": "ben@example.com",
"title": "",
"status": "Active",
"company": "Carter Homes",
"numberOfEmployees": 0,
"industry": 0,
"annualRevenue": 0,
"website": "",
"phone": "",
"mobilePhone": "",
"timezone": "",
"avatarPath": "none",
"country": "",
"city": "",
"postalCode": "",
"address": "",
"geoCode": "32.8462546,-97.1137307",
"dateFirstSeen": "1753-01-01T00:00:00",
"dateLastSeen": "1753-01-01T00:00:00",
"region": "",
"gender": 10,
"dateBirth": null,
"age": 0,
"extendedProperties": {
"eligibility_date": "",
"group_code": "",
"product_code": "",
"source": ""
},
"dateContactCreated": "2018-07-17T00:00:00",
"timestampCreated": "2018-07-17T16:01:44.717",
"dateContactLastModified": "2018-07-17T20:00:12.023",
"dateLastContacted": "2018-07-17T20:00:12.023",
"accountId": 0
},
"id": "1359c31a651f4684a04c6e9d12ec154d"
}
}
</pre>

<ol class="api"><li value="POST">/API/Contact</li></ol>

The `POST` method of `/API/Contact` is used to create or update a Contact.

> If you intend to update multiple records, use `/API/Contact/Import` (see below)

### Sample request body
The body of the POST must include a JSON representation of the Contact. The only field that is required is an email address:

<pre class="brush: javascript">
{
"email": "api@example.com"
}
</pre>

### Request body fields
<table class="table">
<thead>
<tr>
<th>Field</th>
<th>Description</th>
<th>Format</th>
<th>Required</th>
</tr>
</thead>
<tbody>
<tr>
<td>email</td>
<td>The email address of the contact.</td>
<td>string</td>
<td>Yes</td>
</tr>
</tbody>
</table>

When creating a contact the following fields can also be specified.

> Important - if you are updating an existing lead, these fields will be ignored. Instead you will need to use the Contact API to update fields for an existing Contact.

<table class="table">
<thead>
<tr>
<th>Field</th>
<th>Description</th>
<th>Format</th>
<th>Required</th>
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
<td>string</td>
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

To specify additional data, such as custom fields, use `extendedProperties`. For example, if a customer downloaded your mobile app from the Apple App Store.

<pre class="brush: javascript">
{
"email": "api@example.com"
"extendedProperties": {
"appStore": "Apple",
"downloaded": "2018-07-26T00:18:02.623"
}
}
</pre>

Custom data added to `extendedProperties` is part of the Contact and can be used for segmentation and search for enterprise customers. All customers can use custom data for personalization.

<ol class="api"><li value="DELETE">/API/Contact/[DSID]</li></ol>

Sending a `DELETE` request with the DSID of the Contact you wish to delete. Once a Contact is deleted it is ineligible for any DailyStory workflows or camapigns.

> Contacts are deleted, but are not removed from DailyStory immediately.

## API Contact RegisterDevice
The `/API/Contact/RegisterDevice` API is used to register multiple devices (iOS or Android) for Contacts to receive push notifications. Push notifications are configured as part of a Campaign's Workflow.

> *Important* before using the RegisterDevice API you must have configured a [Twilio Notify Service](/integrations/twilio).

<ol class="api"><li value="POST">/API/Contact/RegisterDevice</li></ol>

The `POST` method of `/API/Contact/RegisterDevice` is used to register either an Apple or Android device with a Contact. If multiple devices are registered to the same user, simply call this API with each of the unique device ids.

### Sample request body
The body of the POST must include a JSON object that identifies the `device_type`, `device_id`, and the Contact's `DSID`:

<pre class="brush: javascript">
{
"device_type" : "ios",
"device_id" : "abcdefgh1234567890",
"dsid" : "1234567890"
}
</pre>

### Request body fields
<table class="table">
<thead>
<tr>
<th>Field</th>
<th>Description</th>
<th>Format</th>
<th>Required</th>
</tr>
</thead>
<tbody>
<tr>
<td>device_type</td>
<td>Indicates the type of device</td>
<td>`ios` or `android`</td>
<td>Yes</td>
</tr>
<tr>
<td>device_id</td>
<td>The unique device id</td>
<td>String</td>
<td>Yes</td>
</tr>
<tr>
<td>dsid</td>
<td>The Contact's unique DailyStory Id</td>
<td>String</td>
<td>Yes</td>
</tr>
</tbody>
</table>

### Sample response body
Returns `200 OK` when created.

<pre class="brush: javascript">
{
"Status": true,
"Message": "",
"Code": 200,
"Response": {}
}
</pre>

## API Contact Import
The Contact Import API is designed for bulk importing/updating of contacts. A `POST` to the API is identical to `/API/Contact`. However, the Import API does not return the `DSID` of newly created Contacts as there are created in bulk.

> If a contact already exists, the contact is updated with any new values.

<ol class="api"><li value="POST">/API/Contact/Import</li></ol>

### Sample request body
The body of the POST must include a JSON representation of the Contact. The only field that is required is an email address:
	
<pre class="brush: javascript">
{
	"email": "api@example.com"
}
</pre>

See the `/API/Contact` for additional request body fields.

### Sample response body
Returns `200 OK` when created. Unlike the `POST:API/Contact`, the bulk import does not return the `DSID` of the contacts created.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {}
}
</pre>

> A successful response indicates that the contact is queued for bulk import.