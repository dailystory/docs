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

### Campaign
<table class="table">
<tbody>
<tr>
<td><strong>Path</strong></td>
<td><strong>Verb</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/campaign/#api-campaign">/api/campaign/</a></code></td>
<td>GET, POST, DELETE</td>
<td>Get, create, or delete a campaign.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/campaign/#api-campaign-list">/api/campaign/list</a></code></td>
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
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/">/api/contact</a></code></td>
<td>GET, POST, DELETE</td>
<td>Get, create, or delete a contact.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/#api-contact-registerdevice">/api/contact/registerdevice</a></code></td>
<td>POST</td>
<td>Register a device for a contact for push notifications.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/contact/#api-contact-import">/api/contact/import</a></code></td>
<td>POST</td>
<td>Used for high volume contact import.</td>
</tr>
</tbody>
</table>

### Lead
<table class="table">
<tbody>
<tr>
<td><strong>Path</strong></td>
<td><strong>Verb</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/lead/">/api/lead</a></code></td>
<td>GET, POST, DELETE</td>
<td>Get, create, or delete a lead.</td>
</tr>
<tr>
<td width="25%" nowrap><code><a href="https://docs.dailystory.com/api/lead/#api-lead-list">/api/lead/list</a></code></td>
<td>GET</td>
<td>Returns a paged list of all leads.</td>
</tr>
</tbody>
</table>

## WebHooks
