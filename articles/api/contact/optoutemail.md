{
	title: 'DailyStory Contact REST API / Optout Email',
	description: 'Documentation for DailyStory\'s Contact REST API for opting out of email'
}
# Contact REST API
Use the Contact REST API to create, update or delete Contacts.

## Optout Email
The Contact `/api/v1/contact/optout/email` is used to opt contacts out of non-transactional email sent by DailyStory.

The API accepts both a DsID or an email address.

### POST
Use the HTTP POST verb to post a JSON object to the `/api/v1/contact/optout/email`.

### Sample request body
The body of the POST must include a JSON array containing objects with either an email or a DsID property:

<pre class="brush: javascript">
[{
	"email": "optmeout@example.com"
},{
	"dsid": "eb6a2fbb594143b7b89a2bfc0a8a20b5"
}]
</pre>

### Request body fields
<table class="table">
<thead>
<tr>
<th>Field</th>
<th>Description</th>
<th>Format</th>
</tr>
</thead>
<tbody>
<tr>
<td>email</td>
<td>The email address of the contact.</td>
<td>string</td>
</tr>
<tr>
<td>dsid</td>
<td>The unique DailyStory id (DsId) of the contact.</td>
<td>string</td>
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