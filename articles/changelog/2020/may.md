{
	title: 'May 2020 Product Update',
	description: 'Product Updates for May 2020'
}
# DailyStory Product Updates for May 2020
## May 15, 2020
* convert search to use POST vs GET due to exceeding querystring length of 2048
* bug with event wire up for paging prev/next
* bug in segment members including old model reference
* updates for roles for access control

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
