{
	title: 'DailyStory Push REST API',
	description: 'Documentation for DailyStory\'s Push REST API'
}
# Push Notifications REST API
Use the Push REST API to list, send and manage Push Notifications.

## List
The List API to list all of the Push Notifications available within a campaign.

<ol class="api"><li value="GET">/API/Push/List/[Campaign Id]</li></ol>

Send a `GET` request with the id of the Campaign whose Push Notifications messages to retrieve.

### Sample response body
Returns `200 OK` when created. The body of the response includes a JSON object with additional data with an array of Push Notification messages.

<pre class="brush: javascript">
{
    "Status":true,
    "Message":"",
    "Code":200,
    "Response":
        {
            "messages":[{
                "title":"Anna we're running a special",
                "message":"Get 25% off with the coupon code: DailyStory Today",
                "previewUrl":"https://dsblobus.blob.core.windows.net/ghg0ctulvdx7bu10/assets/asset-PushNotification-1-rg27.png",
                "messageId":1,
                "tenantId":112,
                "campaignId":69,
                "total_sent":42,
                "status":"Active",
                "isEnabled":true
            }]
        }
}
</pre>

## SendSingle
The SendSingle API is used to send a single Push Notification message to a Contact.

<ol class="api"><li value="POST">/API/Push/SendSingle</li></ol>

### POST parameters

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
<td>dsid</td>
<td>The unique DailyStory id of the contact</td>
<td>string</td>
<td>Yes</td>
</tr>
<tr>
<td>title</td>
<td>The title of the Push Notification message</td>
<td>string</td>
<td>Yes</td>
</tr>
<tr>
<td>body</td>
<td>The body of the Push Notification message</td>
<td>string</td>
<td>Yes</td>
</tr>
</tbody>
</table>

If you do not have a DailyStory id (DSID), use the [Contact API](/api/contact) to look up the DSID.

### Sample response body
Returns `200 OK` when sent.

<pre class="brush: javascript">
{
"Status": true,
"Message": "",
"Code": 200,
"Response": {}
}