{
	title: 'December 2017 Product Update',
	description: 'Product Updates for December 2017'
}
# December 4, 2017
* Click through on Email Summary reports

# December 2, 2017
Big update to the APIs mainly for supporting Zapier, but applies to custom REST and WebHooks too.

* Send correct HTTP status codes and JSON codes for bad requests in API
* Updated api/campaign/list to use ApiResponse wrapper
* Update api/lead/list to use paged response
* Added api/linktracking/clicks
* Fix bug in EmailSummaryReport when no results are found
* Updated LinkTracking queue to send webhook events
* Updated ProcessTrigger queue to send webhook events
* Updated ProcessWebhooks to send new message types
* Add PageVisit and LinkClick webhook events
* Refactor ApiStatusReponse
* Add async GetCampaign option
* Add LinkTrackingClick for return in APIs
* Refactor PageViewTrigger for APIs
* 