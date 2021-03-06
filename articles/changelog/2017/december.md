{
	title: 'December 2017 Product Update',
	description: 'Product Updates for December 2017'
}
# December 20, 2017
* Better/faster updates for lead stats
* Lookup for recently added leads
* Ignore Link Tracking with HEAD requests
* Campaign reporting improvements
* Bulk write to storage for web stats

# December 18, 2017
* Added some better handling for adding removing leads to a campaign in bulk
* Added some better handling for adding removing contacts to a list in bulk
* Refactored List Array building out of stored procedure
* Added REST API for managing leads /api/campaign/leads
* Added some conditions for list 0 (all)
* Added some checks for list management
* Updated contact, list and campaign javascript libraries for handling edge conditions around select all
* Small fix to accounts
* Moved JavaScript from Leads.cshtml to separate javascript file
* Updated leads table for UX
* Added classes to paged leads UX for reference in select all javascript

# December 15, 2017
* Added Lists functionality for managing groups of contacts
* Added export for contact lists
* Add support for add all contacts
* Add to Campaign Wizard
* Contact List APIs
* Support for GMail style select all of checkboxes on contacts
* Search defined add/remove lists
* More functional buttons for add/edit with drop down options
* Added /update on Update Search to support adding an index
* Fixed bug in add lead when contact was bounced
* Added HasMoreResults to paged list and dictionary
* Added List property to Contact Document for tracking member lists

# December 13, 2017
* Removed the trial data
* Found an edge case bug in lead creation
* UX cleanup
* Added welcome pane for new users
* Drop downs on main menu for quick actions
* Added validation check when creating new leads that a campaign is set

# December 12, 2017
* Add some async, including LeadModel
* Update Contact export to use search filter
* Refactor and improve manual lead creation UX
* Handle some minor bugs
* Hide fields in Leads and Contact with no data
* Add search support to Leads
* Improve page descriptions and formatting
* Performance improvement to Process Workflows
* Webhook event job needs to run continuously
* Fix Extended Properties condition where could be null
* Fix bug in bounced calculation that was summing the wrong column
* Don't create leads for previously bounced contacts
* Fix bug in Campaign Conversion report
* Added search field management to Contact Document and added sortable to fullname

# December 11, 2017
* Added API key management
* Added /api/lead/activity api for Zapier
* Added license contraint for api key creation
* Addressed UX issues with campaign list
* Misc UX improvements
* Added notification lead activity type for handling unknown activity types
* Fixed some broken links

# December 10, 2017
* Refactored some methods for async to improve throughput
* Fixed Campaign Email report
* Fixed bug in export controller
* Fixed bug in lead detail for search link
* Pass through Leads unit tests
* Updated campaign workflow so when a new step is added existing leads receive that workflow

# December 8, 2017
* Updated email reports to return leads vs contacts
* Added support for Export List of leads in export controller
* Fix bug in EmailCarrd
* Added Email Click actvity type
* Updated Lead Created activity type
* Added Tracking LInk activity type
* Changed references of Account to Company
* Fixed UX issue in page leads to include comma in thousands
* Update to campaign stats 
* Converted lead stats bounced update to use sproc
* Changed look up ip address job to flag contacts for search update
* Updated Email Click Open handling to ignore test leads
* Mailgun integration no longer fetches clicked open, DailyStory handles
* Better exception descriptions for Emails
* Added EmailClick to represent logged email click activities
* Updated LeadActivtity Report to include email clicks and tracking link clicks
* Added Link Tracking Activity
* Fixed calculation bug in Campaign Conversion Report
* Removed some dead wood
* Email Summary Report returns leads
* Update to search to support lookup by field name and friendly formatting
* 
# December 7, 2017
* Updates for Email Reports
* Improved Lead Stat calculation performanc
* Added aggregates for emails to Email object
* Performance improvements for email reporting
* Fixed aggegate calculation bug in Email Summary Report
* 
# December 6, 2017
* Updating lead origination and source display
* Linked Contact and Lead details into search
* Updated activity types
* Updated about API
* Use User Agent for Lead Source for API creation
* Update lead to link into reports
* Update link summary report to include timestamp of click vs. lead activity timestamp
* Corrected some date time stamp issues with emails and link clicks
* Update to home page campaign conversion report
* Include imported metrics in campaign conversion reports
* Friendly search parsing for Contact page
* Add UrlHash to Magic Forms
* Track URL clicks on email clicks

# December 4, 2017
* Click through on Email Summary reports
* Improve dashboard
* Fix bug with Workflow from API changes affecting JavaScript
* Fix bug with Email timestamps for sends
* Improve UX on email reports

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