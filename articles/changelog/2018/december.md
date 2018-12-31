{
	title: 'December 2018 Product Update',
	description: 'Product Updates for December 2018'
}
# DailyStory Product Updates for December 2018
## December 31, 2018
* Refactor: stats properties for segments
* Bug: generate dsid if missing on trial lead
* Refactor: add clear cache option for data manager; mostly for testing purposes
* Refactor: normalize counts in segment stats
* Bug: email activity return name instead of subject
* Bug: set segments in email send task
* Refactor: log more data in text message send queue
* Refactor: remove references to email detail view
* Refactor: comment out add button in schedule
* Initial check-in of segment stats view
* Refactor: thumbnails for text and push
* Refactor: previewurl part of campaign asset
* Bug: email summary report should show if count is > 0
* Refactor: make thumbnail urls not easily guessable
* Feature: support cloning an email

## December 30, 2018
* Refactor: disabled support for syncing optout
* Refactor: contact to track issmsenabled and ispushenabled
* Refactor: removed use of segments bound to email
* Bug: populate from data reader wasn't populating all fields
* Feature: added logic to update segment statistics
* Refactor: log reason when available in sms
* Refactor: handle logging with text messages and undeliverables
* Refactor: handle exceptions in Twilio
* Refactor: return error when debugging
* Refactor: better calculate screen real estate for split editor
* Refactor: iterate on designer for emails
* Bug: hanlde conditions when campaign id is set, but campaign is invalid
* Refactor: trash view with screen shots and click to edit
* Refactor: minor updates to layout

## December 29, 2018
* Refactor: add support for sms counter to calculate segments in message
* Bug: ignore key code for select all

## December 27, 2018
* Bug: all segments in search should be available
* Bug: update segments after saving campaign
* Refactor: added name property to email; changed how inline css for emails is rendered
* Bug: updates for grapesjs css for bigger footer areas in designer
* Refactor: handle passing in search in querystring
* Bug: disable xhtml and enable html on tinyhtml; add copy option
* Bug: don't allow editng of center attribute in designer
* Bug: callbacks to set campaign id on copy; ignore some keyup
* Refactor: add callback when campaign id gets set
* Refactor: updates to views

## December 26, 2018
* Refactor: new bundles for redesigned email, sms and push editors
* Refactor: style updates for new designers
* Refactor: better exception handling in email api
* Refactor: email views updated
* Refactor: multiple updates to views for trash, side menu and more
* Refactor: updates to javascript files for sms, push and emailsa
* Bug: cloning bug with scheduler
* Refactor: adding testing support to scheduler

## December 24, 2018
* Refactor: add description for imports that use a segment
* Refactor: add support for preview url in emails
* Bug: GetEmailsAsync didn't properly filter on status
* Refactor: check if segment have been updated
* Bug: trim text and push messages

## December 20, 2018
* Refactor: update design for confetti message
* Refactor: don't require segment for import
* Feature: screenshots for text and sms
* Refactor: edit option in pages quick menu
* Bug: posted schedule would not return offset timezone
* Refactor: breadcrumb filters to include campaigns
* Bug: _focus template didn't include tool tips library

## December 19, 2018
* Refactor: add support for segments in scheduler
* Refactor: add support for Segments in Campaign API
* Feature: continued updates to scheduler branch
* Refactor: scheduler into components for multiple types
* Bug: LeadOrigin list to segment
* Bug: clone events for email getting published events
* Refactor: support send with filtered segments from schedule
* Bug: typo in date formatter
* Refactor: events to use tags
* Refactor: segments for scheduled push notifications
* Feature: scheduler updates for previews; and segments

## December 18, 2018
* Refactor: Add H2 to message
* Refactor: contacts export emails file for > 5000 contacts
* Refactor: login and trial css
* Refactor: support for queue based export of contacts in tasks
* Refactor: update stats for push notifications
* Bug: edge condition in new tenant creation
* Refactor: clean up scheduled messages
* Bug: campaign stats check for invalid campaign id
* Refactor: update send test push to include title and body

## December 17, 2018
* Refactor: GetScheduleAsync doesn't need message type
* Refactor: add API to schedule controller for listing schedule
* Refactor: move scheduling UX to library

## December 15, 2018
* Refactor: move campaignstats functions into core
* Refactor: update reports to aggregate push and sms
* Refactor: update sparkline reports
* Refactor: update sparkline and reports on campaign detail

## December 14, 2018
* Bug: better error message in contact detail when attempting removal from dynamic segment
* Refactor: improve performance of adding leads to campaign
* Bug: Update campaign could remove segments; refactor add to campaign
* Refactor: tasks for background segment to campaign
* Refactor: LeadQueueItem for ProcessLeads job
* Refactor: added UpdateModifiedIfExists for better lead insert performance
* Refactor: SaveAsync on Lead for better performance

## December 13, 2018
* Bug: advanced search may contain && which caused errors
* Bug: remove leads should reset lead table UX
* Bug: push bindings tool was not using index for display
* Refactor: move register device logic into PushNotifications
* Bug: segments to update filter
* Refactor: handle remove segement from campaign
* Refactor: RegisterDeviceAsync in Push Notifications
* Bug: handle string arrays when rebuilding from contact doc

## December 11, 2018
* Refactor: social media set has posted
* Refactor: segments update campaign on save
* Bug; don't show url in events that have published
* Refactor: campaign rulesets based on unit tests
* Refactor: segments
* Refactor: social media posts
* Refactor: clean up campaign API

## December 10, 2018
* Update project library dependencies
* Refactor: media calendar
* Bug: MindBody extended properties could get overwritten
* Refactor: updates to campaign cloning
* Bug: check if contact is enabled for push
* Bug: search filter for non-field types
* Refactor: scheduled messages send push notifications
* Refactor: timezone offset managed internal to class
* Bug: import contact should use safe get/set for extended properties
* Bug: set tenant id in segment export

## December 8, 2018
* Feature: add push notification and text message applications
* Feature: SmsActivityItem
* Refactor: updates to schedule of events
* Refactor: updates to scheduled messages for SMS and push
* Bug: fixes to lookup ip address
* Add: SyncTwilio job for sending/queuing SMS and Push
* Add: css for full calendar
* Add: schedule controller to add/remove items to schedule
* Refactor: return test messages as a campaign asset
* Add: model for campaign scheduler
* Refactor: return to opening page on contact save & close
* Refactor: add button to create a segment on contact search
* Bug: email scheduler formatted date incorrectly
* Bug: better handle dynamic search that doesn't start with s=
* Refactor: campaign assets list text messages
* Feature: campaign schedule
* Update: views with new features

## December 6, 2018
* Refactor: bettter navigation on save & close
* Refactor: add description to segment list
* Bug: avatar path shouldn't be overwritten in contact merge
* Refactor: added events and date filter item to handle specific date filtering

## December 5, 2018
* Refactor: UX improvements and updates
* Feature: add support for contact avatar display
* Refactor: better batching for removing leads from a campaign
* Refactor: add check for workflows in campaign and improve performance of remove leads
* Feature: added GeoIPData with ipstack
* Bug: handle nulls in IpInfo
* Refactor: set workflowId on lead to 0 if campaign does not have a workflow
* Refactor: segment export
* Refactor: simplify wait until calculation
* Bug: old reference to segments
* Feature: add support for events

## December 3, 2018
* Refactor: contact list to segment
* Refactor: expanded graph fields on ContactDocument

## December 2, 2018
* Refactor: responsive updates
* Bug: validation error in segment javascript
* Bug: new segments created with bad last modified timestamp
* Refactor: search filters updated

## December 1, 2018
* Refactor: add UX for bool types in advanced udf search
* Refactor: add BoolSearchFilter for search filters
* Bug: test segment should open in new tab or popup
* Bug: typo in bootstrap hidden xs usage