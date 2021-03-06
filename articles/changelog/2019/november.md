{
	title: 'November 2019 Product Update',
	description: 'Product Updates for November 2019'
}
# DailyStory Product Updates for November 2019
## November 30, 2019
* Refactor: add geocode lookup for Telligent sync
* Bug: title width could force buttons off screen
* Refactor: add route for open rate stats
* Refactor: add email data science
* Refactor: update email reports and add delivered

## November 28, 2019
* Refactor: magic form status ux
* Refactor: Task status ux
* Refactor: Seggment status logic
* Refactor: standard delete
* Bug: catch exceptions when trying to load remote pages for preview
* Bug: update and fix issues with visit alerts ux
* Refactor: pause and reactivate visit alerts
* Refactor: code clean up Page View Triggers

## November 27, 2019
* Refactor: remove old get emails
* Refactor: get assets return active or paused
* Refactor: argument check for isstatus
* Refactor: filter status
* Bug: schedule view should return campaign of any status
* Bug: popup name in list should be link
* Refactor: better UX for campaign state
* Refactor: campaigns in archive
* Refactor: Link Tracking status
* Refactor: tracking links menu with reports
* Refactor: display link tracking paused
* Refactor: popup status ux
* Refactor: popup menus
* Refactor: segment status ux

## November 26, 2019
* Refactor: update error messages
* Bug: format total members and remove model
* Bug: segment name as link
* Refactor: use view for segment stats
* Refactor: scheduled messages by utc date
* Refactor: segments updated to use views

## November 25, 2019
* Refactor: normalize file manager create and add folder
* Refactor: contacts to support ajax loading
* Refactor: add server-side sorting for segments
* Refactor: process task queue
* Refactor: force utc date check
* Refactor: perf improvements and bugs with segment rebuilding
* Refactor: smaller parallel task queue

## November 24, 2019
* Refactor: segments api
* Refactor: add SkipList
* Refactor: remove paged api for segments
* Refactor: ajax datatable for segments
* Refactor: api for skip and take segments
* Refactor: update segments ux

## November 23, 2019
* Refactor: updates to campaign
* Bug: owneruid on campaign null check
* Refactor: code cleanup
* Refactor: create task if campaign has owneruid
* Bug: campaign menu was off
* Bug: remove search on dashboard
* Refactor: web form index menu
* Refactor: updates to webforms
* Refactor: add support for segments converted

## November 22, 2019
* Refactor: popup clone logic
* Refactor: handle delete through api
* Refactor: campaign ux
* Refactor: popup clone logic
* Refactor: handle delete through api
* Refactor: add change status for campaign

## November 21, 2019
* Bug: tenantuid not set properly
* Bug: support old api route
* Refactor: remote only errors
* Refactor: popups disabled when _dsTrack only is true
* Bug: minify caused evaluation of null object in magic form scripts
* Refactor: convert Telligent plug-in to use versioned api
* Bug: long title could force buttons to wrap in designer

## November 20, 2019
* Refactor: set lead source in submitted forms
* Refactor: add route maps
* Refactor: convert to use lead queue
* Refactor: SetLeadSource id
* Refactor: undo origin for web form
* Bug: search birthdate returned wrong format
* Refactor: add support for source to contact document
* Refactor: set source in lead for popup

## November 19, 2019
* Refactor: tracking type for webform
* Refactor: formatting
* Refactor: email address exception handling to change contact status
* Refactor: add EmailAddressException
* Refactor: highlight message for test message user
* Bug: email activity item can be null
* Refactor: change how mailspools handle exceptions
* Refactor: api contact controller
* Bug: push controller needs to support json body

## Nobember 18, 2019
* Bug: clone name should be public
* Bug: update stripe versions to get around immutables error
* Refactor: update to new Stripe
* Refactor: add support for start end automation

## November 17, 2019
* Refactor: campaign; build errors add support for start end
* Refactor: fix build messages
* Refactor: remove contactlistmember
* Refactor: fix build message and modernize
* Refactor: update stripe
* Refactor: update segments
* Refactor: bug in whitelabel image width
* Refactor: add support for start end date in campaigns
* Refactor: remove contact list members in segment partial
* Refactor: update for campaign api routes
* Refactor: add support for campaign start/end ux
* Bug: set start end when cloning campaign
* Refactor: update search packages

## November 13, 2019
* Refactor: clean up tasks js files
* Refactor: allow from cache flag for tasks
* Refactor: d37 sync regardless of last sync time
* Refactor: campaign apis
* Refactor: address compiler warnings for campaigns
* Refactor: update description
* Refactor: campaigns for active and paused views
* Refactor: filter status on campaigns

## November 12, 2019
* Refactor: MINDBODY online icon
* Bug: send emails needed negative minutes back
* Refactor: heatmaps on separate bullet in reports
* Refactor: support recently sent emails
* Refactor: adjust back button font in login.css
* Refactor: set default calendar view to week
* Refactor: main event calendar filtered to today
* Refactor: color highlight calendar
* Bug: fix issues to support mce 5
* Refactor: switch mindbody icon
* Refactor: about api
* Refactor: task css
* Refactor: remove tasks archive
* Refactor: tasks menus and selections

## November 11, 2019
* Bug: slug could get set to empty string
* Bug: LeadQueue must specify data center
* Refactor: set RedirectUrl to empty if message is action type
* Refactor: stub function for generating secret proof in Facebook
* Refactor: convert from sproc
* Bug: web forms should only return active
* Refactor: add email instrumentation
* Refactor: update MBO sync hourly
* Refactor: email instrumentation to handle better granularity
* Refactor: update graphs automatically
* Refactor: update instrumentation routes
* Refactor: side bar menu as partial
* Refactor: more updates to email instrumentation
* Refactor: use utc for moment.js
* Refactor: json dates handling for reports
* Bug: timezones in email instrumentation

## November 10, 2019
* Refactor: updates to instrumentation

## November 8, 2019
* Refactor: enable webform with embedded message
* Bug: allow access control origin

## November 7, 2019
* Refactor: schedule.js to bubble error messages
* Bug: check if campaign is valid before scheduling
* Refactor: opt out of parent if contact in child unsubscribes
* Refactor: GetStatsAsync for campaign
* Refactor: email instrumentation
* Bug: handle nulls for campaign stats
* Refactor: warn when there are no leads in the campaign

## November 6, 2019
* Refactor: async campaign lookup
* Bug: handle case where title and body html are empty
* Bug: set slug if not specified
* Bug: exported popup is active
* Refactor: add GetStatsAsync to campaign for API
* Refactor: api namespace
* Refactor: campaign api
* Refactor: convert auto archive to sproc
* Refactor: update libs for cms
* Refactor: update mailgun spools

## November 5, 2019
* Refactor: don't set button target for pages
* Bug: updates to preheader

## November 4, 2019
* Refactor: display errors when creating trial
* Refactor: better handle error messages
* Bug: ignore emails with a test dsid for status