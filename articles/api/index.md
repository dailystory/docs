{
	title: 'DailyStory SDK and API Documentation',
	description: 'Documentation for DailyStory\'s SDKs and APIs'
}
# DailyStory SDKs and APIs
DailyStory includes a full suite of REST APIs and WebHooks for integrating and extending the DailyStory platform.

The [open source and published on GitHub](https://github.com/dailystory/SDKs/) provide developers with pre-built libraries that make it easy to integrate your application with DailyStory. The REST APIs and WebHooks provide more extensive integration opportunities.

> If you are integrating DailyStory into your existing application you may want to investigate our [Zapier Triggers and Actions](https://zapier.com/). Zapier makes it easy to create workflows without requiring developers.

## Software Development Kits (SDKs)
The DailyStory SDKs are [open source and published on GitHub](https://github.com/dailystory/SDKs/). There are currently two published SDKs.

* SDK for .NET Developers
* SDK for PHP Developers

### SDK for .NET Developers
The [SDK for .NET Developers](/sdk/dotnet) is an [open source library hosted on GitHub](https://github.com/dailystory/SDKs/tree/master/DotNet) used by .NET developers to integrate DailyStory's capabilities into their .NET application.

### SDK for PHP Developers
The [SDK for PHP Developers](/sdk/php) is an [open source library hosted on GitHub](https://github.com/dailystory/SDKs/tree/master/PHP) used by PHP developers to integrate DailyStory's capabilities into their PHP application.

## REST APIs
All of DailyStory's platform is accessible through a REST API and WebHooks for receiving notification about events.

> Important, our API documentation is not complete. If you are looking for an API or WebHook that isn't in the documentation, please [contact us](https://dailystory/contact-us) and we'll add it.

* [About](/api/about)

### Campaign
<table class="table">
<tbody>
<tr>
<td><strong>Path</strong></td>
<td><strong>Verb</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/campaign/#api-campaign">/api/v1/campaign/</a></code></td>
<td>GET, POST, DELETE</td>
<td>Get, create, or delete a campaign.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/campaign/#api-campaign-list">/api/v1/campaign/list</a></code></td>
<td>GET</td>
<td>Returns a list of active campaigns.</td>
</tr>
</tbody>
</table>

### Contact
<table class="table">
<tbody>
<tr>
<td><strong>Path</strong></td>
<td><strong>Verb</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/">/api/v1/contact</a></code></td>
<td>GET, POST, DELETE</td>
<td>Get, create, or delete a contact.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/#api-contact-registerdevice">/api/v1/contact/registerdevice</a></code></td>
<td>POST</td>
<td>Register a device for a contact for push notifications.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/#api-contact-import">/api/v1/contact/import</a></code></td>
<td>POST</td>
<td>Used for high volume contact import.</td>
</tr>
</tbody>
</table>

### Lead

* [**GET /api/v1/lead**](/api/lead/) - get a lead by id
* [**DELETE /api/v1/lead**](/api/lead/) - delete a lead by id
* [**POST /api/v1/lead**](/api/lead/) - create or update a lead
* [**GET /api/v1/leads**](/api/lead/) - returns a paged list of all leads

### Push Notifications

* [**GET /api/v1/pushnotification**](/api/push/) - get a push notification by id
* [**DELETE /api/v1/pushnotification**](/api/push/) - delete a push notification by id
* [**POST /api/v1/pushnotification**](/api/push/) - create or update a push notification
* [**GET /api/v1/pushnotifications**](/api/push/) - get all push notifications
* [**POST /api/v1/pushnotification/sendsingle**](/api/push#sendsingle) - send a single push notification
