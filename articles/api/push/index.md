{
	title: 'DailyStory Push REST API',
	description: 'Documentation for DailyStory\'s Push REST API'
}
# Push Notifications REST API
Use the Push REST API to list, send and manage Push Notifications.

## Push
The `Push` API is used to create or update a Push Notification `POST`, retrieve a push notification `GET`, or delete a push notification `DELETE`.

<ol class="api"><li value="GET">/api/v1/push/[ID]</li></ol>

The `GET` method of `/api/v1/push/[ID]` is used to retrieve an existing Push Notification. The `[ID]` is the id of the Push Notification to retrieve.

To see this in action, [login to DailyStory](https://app.dailystory.com/login) and navigate to an existing Push Notification. For example, `/Push/Edit/1`. Then change the URL to `api/v1/push/1` to see the JSON representation.

### Sample response body
Returns `200 OK` when created. The body of the response includes a JSON object with additional data with the `id` of the Push Notification.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {
        "message": {
            "title": "Anna we're running a special",
            "message": "Get 25% off with the coupon code: DailyStory Today",
            "previewUrl": "https://dsblobus.blob.core.windows.net/ghg0ctulvdx7bu10/assets/asset-PushNotification-1-rg27.png",
            "messageId": 1,
            "tenantId": 112,
            "campaignId": 69,
            "total_sent": 86,
            "status": "Active",
            "isEnabled": true
        },
        "id": "1"
    }
}
</pre>

<ol class="api"><li value="POST">/api/v1/push</li></ol>

The `POST` method of `/api/v1/push` is used to create or update a Push Notification.

### Sample request body
The body of the `POST` must include a JSON representation of the Push Notification:

<pre class="brush: javascript">
{
    "title": "Anna we're running a special",
    "message": "Get 25% off with the coupon code: DailyStory Today",
    "previewUrl": "https://dsblobus.blob.core.windows.net/ghg0ctulvdx7bu10/assets/asset-PushNotification-1-rg27.png",
    "messageId": 1,
    "campaignId": 69,
    "status": "Active",
    "isEnabled": true
}
</pre>

> To create a new Push Notification either omit the `messageId` or set it to 0.

### Sample response body
The `POST` method returns a JSON object along with the id of the Push Notification that was either created or updated.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {
        "id": "1"
    }
}
</pre>

The `DELETE` method of `/api/v1/push/[ID]` is used to delete a Push Notification. The `[ID]` is the id of the Push Notification to delete.

> Deleted Push Notifications are moved to the Trash.

### Sample response body
The `POST` method returns a JSON object along with the id of the Push Notification that was either created or updated.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {
    }
}
</pre>

## All Push Notifications
Use the `/pushs/` API to list all of the Push Notifications available.

<ol class="api"><li value="GET">/api/v1/pushs/</li></ol>

Optionally filter by a specific campaign:

`/api/v1/pushs/?campaignId=[Campaign Id]`

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

## Send Single <a name="#sendsingle"></a>
The SendSingle API is used to send a single Push Notification message to a Contact.

<ol class="api"><li value="POST">/api/v1/push/sendsingle/[DSID]</li></ol>

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

### Sample request body
<pre class="brush: javascript">
{
    "title": "test push title",
    "body": "test push body",
}
</pre>

### Sample response body
Returns `200 OK` when sent.

<pre class="brush: javascript">
{
    "Status": true,
    "Message": "",
    "Code": 200,
    "Response": {}
}
</pre>

> A 200 OK response from the API only means that the Push request was succesfully accepted and queued for delivery.