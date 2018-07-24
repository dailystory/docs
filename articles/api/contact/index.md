{
	title: 'DailyStory Contact REST API',
	description: 'Documentation for DailyStory\'s Contact REST API'
}
# Contact REST API
Use the Contact REST API to create, update or delete Contacts.

## API Contact Import
The Contact Import API is designed for bulk importing/updating of contacts.

> If a contact already exists, the contact is updated with any new values.

<ol class="api"><li value="POST">/API/Contact/Import</li></ol>

### Sample request body
The body of the POST must include a JSON representation of the Contact. The only field that is required is an email address:
	
<pre class="brush: javascript">
{
	"email": "api@example.com"
}
</pre>

To see all the available fields [login to DailyStory](https://app.dailystory.com/login) and navigate to an existing contact. For example, `/Contact/Detail/1359c31a651f4684a04c6e9d12ec154d`. Then change the URL to `API/Contact/1359c31a651f4684a04c6e9d12ec154d` to see the JSON representation.

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

Custom data added to `extendedProperties` is part of the Contact and can be used for segmentation and for enterprise customers, search.

## Sample response body
Returns `200 OK` when created. The body of the response includes a JSON object with additional data with the `Id` of the Lead.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {}
}
</pre>

> A successful response indicates that the contact is queued for bulk import.