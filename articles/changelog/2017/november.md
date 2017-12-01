{
	title: 'November 2017 Product Update',
	description: 'Product Updates for September 2017'
}
#November 30, 2017
* Email delivery report with opens, clicks, and bounces
* Email optout report
* API /about end point
* Refactor Campaign controller for better performance
* Convert bulk import to use field map json file
* Add EmailReports
* Add Email Summary Report
* Add optout report to navigation
* Update LeadStats job to not use MailGun stats for opened or clicked
* Refactor EmailRedirectQueue job to handle clicks and opens for emails
* Update MailGun integration to ignore opens and clicks
* Add event webhooks for Zapier support
* Add ContactMapFile for better bulk import support on background jobs
* Refactor license to allow for overriding default license limits
* Refactor CampaignEmailReport and Add EmailSummaryReport
* Update WebTrackingCallback to use queues to track email opens

#November 28, 2017
* Added support for Zapier triggers and actions beta
* Refactor the API namespace
* Add support for event webhooks for Zapier and other developers
* Add support for PagedApiStatusResponse for paged responses from the API
* Changed Do Not Contact to a toggle option and refactored
* Added support for event webhooks when new lead is created
* Added h:sender header for better MailGun on behalf of support
* Initial check-in of WebhookEventQueue job
* Api for subscribe/unsubscribe to webhook events. Mainly for Zapier for now
* Added List api to api/lead
* Fixed bug in opt-out
* Changed opt out behavior in contact to use toggle button
* Changed bulk import to background process

#November 26, 2017
* Fix bug with description serialization on forms
* Refactor and clean up jobs
* Fix bug in unsubscribe from lead notification emails
* Initial updates for Zapier support
* Bug with reseting DsId from querystring
* Support for Zapier Trigger web hooks

#November 15, 2017
* Conversion events are highlighted better on the lead timeline
* Reports export controller handles Lead Extended Properties
* Add support for textareas on Magic Forms
* Add support for assets section of campaigns to quickly see which DailyStory features are used
* Add support for custom fields on webforms
* Add support for Campaign listing in Popups, Content Pages, Magic Forms, Pay per click, 
* Add full url property to Content Pages for editing
* Add support for ICampaignAsset to Emails, Link Tracking, Magic Forms, Popup, Web Form
* Reverse sort the web activity items for leads so page views are old > new
* Update link tracking queue item insert to use creation date vs execution date
* Bug in campaign ruleset with id management
* Fix encoding bug for admin editing in Google Analytics

# November 13, 2017
* Http Verb tracking for redirects
* Fix bug in encoding for Google Analytics in UX
* Fix bug in trial setup

# November 11, 2017
* Fix bug in Magic Form location parsing
* Better error logging for general exceptions
* Bug in Popup reports from refactor

# November 10, 2017
* Refactor popups
* Better log handling to prevent log flooding
* Better ordering for link quick menu items
* Fix HTML encoding issues with Google Analytics tag integration
* Update content pages to use Google Analytics tags and remarketing tags

# November 9, 2017
* Updated all jobs to use connection provider environment variables
* Added more tests for jobs
* Move automation rules processing to its own job
* Added RunAutomations job
* Better exception handling/logging for Salesforce
* Changed Salesforce sync to only occur on lead creation
* Fix for OriginAS parsing in Ip lookup
* Added additional logging for application errors
* Added caching for campaign rule sets as part of performance improvements
* Performance improvments to DsJsonWrapper to prevent cache race condition
* Performance improvements to WebForm lookups
* Better logic for output caching of json and other downstream file types
* Some UX improvements

# November 3, 2017
* Updates to Daily Digest
* Added form type to Web Forms to support data entry use case
* Refactor Lead to removed description from extended properties
* Refactor Lead to use Lead Extended Properties
* Added Admin class
* Added Page Info report and fixed bug in summary report
* Performance improvement to rendered json
* Performance improvements on generated Ds files

# November 2, 2017
* Remove modal campaign selector from link tracking

# November 1, 2017
* Update to Salesforce integration to better support lead field mapping
* Added SalesforceFieldItem to represent the salesforce field data
* Converted Salesforce import to use field item
* Removed some forced properties from the Salesforce object
* Added page for configuring Salesforce settings to App
* Added better support for radio and checkbox input types in Magic Forms
* Added Ux to Lead Detail for extended properties
* Added test link option to inbound/outbound links
* Formatting on IpInfo
* Updates to Lead Queue Item to write into Lead Extensions
* Added clean up to ds_redirect_log to clean up orphaned items
* Fix for Lead Extended Properties