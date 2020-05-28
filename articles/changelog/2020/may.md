{
	title: 'May 2020 Product Update',
	description: 'Product Updates for May 2020'
}
# DailyStory Product Updates for May 2020
## May 28, 2020
* don't set internal email when creating contact from text message keyword
* format number of files in folder
* Refactor file folder asset to handle create updates and re-org code
* update file manager styles
* add support for audit event entries in logs
* updates to audit event logging
* change Twilio sync to run continously
* updates to graph field to use new api
* styles to leads
* ensure optin gets reset properly
* obscure email should accept empty string now that email isn't the only validating property
* adjustments to contact preferences logic to reset enabled state on optin
* clean up formatting for logging
* log credits required per text message
* added logic to handle de-duplicating leads with same number or email when doing queued sends
* update maintenance job
* update to weave integration for location and secret
* bug with file manager too aggresively deleted from storage
* set permanent delete to 30 days

## May 27, 2020
* convert jobs to use async main
* better handling of exceptions when email status is not found
* allow text message lookup with cache skip
* allow email lookup with cache skip
* sync bug with weave to sync on mobile phone when contact not found

## May 26, 2020
* Add report not ready exception
* edits to error messages to make them more user friendly
* bug in pager events with data table
* throw report not ready exception when report is not ready
* include whitelable logo in message
* bug with show/hide data table info
* updates to file manager for better ux
* search files should only include actives

## May 25, 2020
* send from queue pattern similar to emails for text messages
* updates to job manager for non-tenant specific jobs
* refactor how lead activity is resolved

## May 22, 2020
* add service point manager max for twilio
* set prod twilio queue to 120 min 
* refactor for async and getting message queue
* refactor how text message send queue handles bulk sends
* update contacts email if lead email is not internal
* add test user note to text message modal 
* return file count in folders api
* updates to file manager to use apis vs server side

## May 21, 2020
* bugs with web forms create logic
* mark as contacted prior to sending emails
* modify text messages to used batch update for contacted
* add typing interval and search callback to datatable
* handle clear search area and callback on button click for search
* include breadcrumbs span even when no content
* bug with how datatable library handles event wireups
* display mobile phone if email is an internal email and we don't have name

## May 20, 2020
* improve error message when error occurrs from data center account switch
* handle cases where filename cannot be read
* Scheduled message no older than 15 minutes

## May 19, 2020
* update weave to support batch syncing

## May 18, 2020
* convert tracking links to web publish project and fix 404 issue with expired tenants
* add system as supported storage type for data center
* comma separator in totals for autopilot

## May 15, 2020
* convert search to use POST vs GET due to exceeding querystring length of 2048
* bug with event wire up for paging prev/next
* bug in segment members including old model reference
* updates for roles for access control
* bug with custom reply to address field
* fix click and reply rate reports for text messages
* add reportcanview role
* add autopilot blocks for text message clicks
* updates to funnel conversion rates

## May 14, 2020
* updated funnel docs and refactor conversions by campaign
* add funnel lookup by uuid
* move conversion to separate class file in funnel
* add EmailSender for managing list of from addresses
* Add exception if filename exceeds 256 characters
* add support for managing a list of email senders
* add support for handlebars formatdate
* refresh campaign segments after contact import

## May 13, 2020
* initial check in for manage email senders

## May 12, 2020
* perform validation on mobile numbers
* ensure MSO comments are formatted correctly
* updates to license and credit management
* Enable URL hash vs encoded URL in emails
* Replace invalid apostrophes in text message content that aren't ascii
* allow comment in email html body
* handle case where campaign id is null on opt out log
* return license exception error messages
* Handle save and close on html emails when there are no changes
* bug in file manager when progress bar is not in current row's page
* add handle to email designer to retain html comments

## May 10, 2020
* Replace spaces in files when preserving filename
* Attempt to base64 decode u value
* preview MMS in text messages

## May 8, 2020
* search needed to support parentheses for multi value array search
* bug with $ not getting replaces when building the segment
* formatting to support MMS in text message editor
* add support for mediaurl for mms messages in twilio api
* calculate number of credits and include mms cost
* support filtering by file types in file manager
* updates to support MMS text messages
* add media url in sms object

## May 7, 2020
* suport for campaign folders and favorites
* File manager clean up
* Claims check not needed on favorites
* clean up campaign paused, archive, etc
* Lighten paused controller for campaign
* Remove old material icon formatters
* SQL param is not used
* update segment ux
* updates to funnels
* Change height of text message preview area based on content length
* log campaign id with optout information

## May 6, 2020
* autopopulate picklists for Mindbody
* autopopulate picklists for Telligent
* fix formatting issues in Weave sync
* update installer with picklist settings
* autopopulate pick lists for RhinoFit
* add lead status of converted and valid for sending
* convert to use cdn for images
* funnel controls and apis wired into campaigns

## May 5, 2020
* set sort order and group name on weave installer
* support yes/no graph field types
* add support for generation to search
* add support to auto pick list building for salesforce
* update weave installer to support auto update fields
* new fields for weave and support auto picklist updates
* support in cms for forcing page from cache if test user
* add support for funnels
* process funnel on web view
* add support for sort and autoupdate on graph fields
* common method to quickly convert utc to tenant's timezone

## May 4, 2020
* remove check if can run seach
* Updates to segment members to support removing contacts
* add support for campaign tie back in ds scripts
* convert mailgun jobs to always on
* add method for looking up campaign by utm campaign id
* update paths for notifications
* add campaign support to tracking queue item

## May 3, 2020
* fix datetime bug for search ranges
* fix range issue on search with past next ranges
* remove old code in campaign selector

## May 1, 2020
* standardize pager info styles
* responsive css updates
* stub support for add tags in contact list
* support sorting of graph fields
* update settings for job singletons
* only lookup ips for active tenants
* bug in common ux referenced email not segments
* release version of web config for publication
* remove old search navigation
* bug in email edit screen
