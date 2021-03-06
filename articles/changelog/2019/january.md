{
	title: 'January 2019 Product Update',
	description: 'Product Updates for January 2019'
}
# DailyStory Product Updates for January 2019
## January 30, 2019
* Refactor: support for check if has child folders and parent
* Refactor: css updates
* Refacctor: folder creation and selection
* Bug: remove campaign youtube 
* Refactor: load file from common ux

## January 29, 2019
* Bug: assigned to user not set correctly
* Refactor: add support for task edited by
* Refactor: handle change detection in tasks for notifications
* Bug: task create edit needs to use non-enum dropdowns
* Refactor: add task status changed notification
* Refactor: detect status changes in tasks
* Refactor: assigned tasks unit test validation
* Refactor: initial integration class for d37
* Refactor: open on click
* Refactor: fade out completed tasks
* Refactor: add support for navigating folders
* Refactor: add notification for task deleted
* Bug: handle nulls in task comparisons

## January 28	, 2019
* Refactor: better responsive support for tasks
* Refactor: support create folder on upload option
* Refactor: add breadcrumbs for file manager
* Refactor: add select all/none support
* Refactor: style file manager
* Refactor: api to format file counts
* Bug: if member is inactive set memberships to empty
* Refactor: file asset icons
* Bug: handle checkbox click event late binding
* Refactor: add integration for degree37
* Refactor: change asset icon dimensions
* Refactor: GenerateFilenameHash
* Refactor: add file types
* Refactor: work on folder picker

## January 26, 2019
* Refactor: file manager initial check in
* Refactor: add folder support
* Bug: tasks didn't include pager
* Refactor: tasks to use file manager for file storage

## January 25, 2019
* Refactor: UX move email templates into email menu
* Bug: include push asset in campaign list
* Refactor: create template from email
* Refactor: pass tenant in for sub-account creation
* Bug: page controller didn't follow standard save
* Bug: check and set already received messages
* Bug: validate text fields on admin settings should allow blank
* Bug: hide some admin features for white label clients

## January 24, 2019
* Refactor: add permission checks
* Bug: segments click on row wrong id
* Bug: visit alerts error mentioned magic forms
* Bug: css for beautify cannot be null

## January 23, 2019
* Refactor: email templates and email; remove old files
* Refactor: css generator required for email designer
* Refactor: remove notification for email/template save
* Refactor: consistent titles for editors
* Refactor: fix ux padding/layout/headers for designer
* Refactor: set styles for responsive
* Bug: Not found errors could log user out
* Refactor: clone email templates
* Refactor: add urls to graph
* Refactor: email templates support status filtering
* Bug: time picker button in scheduler not working
* Bug: don't post empty notes
* Refactor: css beautify

## January 22, 2019
* Refactor: add support to generate css for emails and templates
* Refactor: add description and css support to emails and templates
* Refactor: update _datatable to support template gallery section
* Refactor: rearrange content menu nav
* Bug: fix path issues in email template
* Bug: cmd-s broken; add support for cssbeautify
* Refactor: add inline css support for email designer
* Refactor: add description and css to email 
* Refactor: allow for empty is valid for url validation
* Refactor: support account urls

## January 21, 2019
* Bug: setused in campaign
* Bug: status not captured
* Add: images for Google play and iOS
* Refactor: drag-and-drop app store icons
* Refactor: svg for app store icons
* Refactor: style updates
* Refactor: tasks updates for bulk edit; date times
* Bug: new tasks should have due and start date today
* Refactor: add link properties to Tenant settings
* Refactor: trigger queue job
* Refactor: create link from not found menu
* Refactor: pass model to activity for contact detail
* Refactor: split out retargeting pixels
* Refactor: move popup field selection inline
* Refactor: test button and display options
* Refactor: update button text
* Bug: fix footer layout

## January 19, 2019
* Bug: visit alerts should use email name not subject
* Bug: race condition with workflow last contacted
* Refactor: update visit alerts
* Refactor: set campaign name through js

## January 16, 2019
* Refactor: add image upload to task
* Bug: workflow should use name instead of subject for emails
* Refactor: associated with selector should use with_id
* Bug: don't show time if time is midnight
* Refactor: format for overdue dates as red
* Refactor: handle midnight as Today, Tomorrow, Yesterday
* Refactor: send notification on assigned task
* Refactor: handle overdue; utc formatting; send notification
* Refactor: update UX for visit alerts
* Refactor: update enum descriptions for visit alerts
* Refactor: add static send for emails
* Refactor: move webstats job logic into core

## January 15, 2019
* Refactor: finalize task branch for merge
* Bug: setting fullname in contact save
* Refactor: bulk edit updates for assigned task
* Bug: handle associated with id and delete
* Bug: missing closing bracket

## January 13, 2019
* Bug: check for associated with nulls
* Refactor: add support for associated with selector
* Refactor: update status ux in tasks
* Refactor: tasks updates for trash, archive, etc.
* Refactor: return current user from users API
* Bug: magic forms edge case bug; added status of form submit wireup
* Refactor: add exception handling to send test sms
* Bug: test lead needed to have IsSmsEnabled to true
* Updates: Assigned tasks
* Refactor: return fullname on contact object
* Bug: text message bad number exception needs to return number
* Refactor: updates to magicforms to handle anchor submits
* Bug: campaign group by caused bad sums
* Bug: fixed message if magic form found

## January 12, 2019
* Add: search api for contacts
* Branch Tasks feature
* Bug: ux layout issues

## January 11, 2019
* Bug: with how relative links, e.g. example.com/#contact are handled

## January 10, 2019
* Add: controllers and javascript for tasks
* Refactor: add support for data and associated with selection
* Bug: magic form could get set to paused

## January 9, 2019
* Refactor: update push with push test from UX
* Refactor: option to ignore active only emails for sending tests
* Bug: support testing for push notification to a contact email
* Bug: fix datetime conversion deprecation warning in scheduler
* Refactor: Send to allow/ignore actives
* Refactor: GetTestLead to support lead from contact
* Add: assigned tasks initial check-in
* Refactor: support personalization in push message title

## January 8, 2019
* Bug: set campaign id on scheduler
* Bug: load segments before loading schedule
* Feature: initial check in for assigned tasks
* Bug: better handle scheduler hide/show

## January 7, 2019
* Bug: don't load please wait if called twice
* Refactor: Magic Forms editor UX
* Bug: Magic Forms references wrong asset type
* Refactor: add support for image preview for Magic Forms
* Feature: Preview URL for previewing images in assets

## January 5, 2019
* Refactor: show date when segment will be deleted
* Refactor: add specific delete api
* Bug: wrong column for delete date stamp
* Refactor: update link tracking api; clean up routes
* Refactor: update link tracking create / edit scripts for delete
* Refactor: update UX for social media
* Refactor: simplify create tracking link
* Refactor: added tutorial videos and fixed bad text
* Refactor: new UX for Magic Forms
* Bug: Magic Forms filter for Active
* Refactor: reponsive updates
* Refactor: add no preview image support

## January 4, 2019
* Refactor: progression on popup conversion to split editor
* Refactor: add preview url support to popup
* Refactor: add in image preview
* Refactor: remove the ability to clone workflows
* Refactor: update cloning and add text message support
* Feature: check if DailyStory tracking tag is installed on page
* Refactor: clean up email validation and cloning
* Refactor: check if tracking tag is installed to determine link direction
* Refactor: move link tracking stats out of job and into core
* Refactor: clean up text message cloning
* Refactor: add support for popups and email templates to thumbnails
* Refactor: set defaults for popup in library
* Obsolete: removing clone in workflows
* Bug: searches that only have filters cause problems saving as segments
* Bug: remove icon column from segments trash view
* Refactor: add undelete to campaign; link to edit not detail from trash
* Refactor: handle remove from trash

## January 3, 2019
* Refactor: update url for events in schedule
* Refactor: remove trigger job from task add to queue (performance)
* Refactor: clean up tracking links
* Refactor: better handle different assets ids in image store
* Bug: lightning context reference
* Refactor: better please wait messages
* Refactor: footer style and confetti message
* Refactor: don't clone workflow
* Refactor: add support for campaign data table
* Refactor: include archive and use titles on pages
* Refactor: campign view
* Bug: cloned emails didn't copy preview url
* Refactor: allow data table sidebar menu to be custom
* Bug: designer title is hardcoded
* Bug: plaintext editor not defined
* Bug: title updates
* Bug: conflicts with #footer
* Bug: old email create links
* Refactor: new UX for managing segments

## January 2, 2019
* Bug: campaigns of type active should include paused
* Bug: timzone offsets for scheduled workflow events
* Bug: scheduler didn't get correct id
* Refactor: move tracking link images to docs