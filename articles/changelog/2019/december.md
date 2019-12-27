{
	title: 'December 2019 Product Update',
	description: 'Product Updates for December 2019'
}
# DailyStory Product Updates for December 2019
## December 27, 2019
* Bug: disable open click segments for now
* Refactor: update logging to use tenant's timezone for dates
* Bug: update for timezones
* Refactor: update email dashboard reports
* Bug: calculate per day and per email
* Refactor: add ctor to report

## December 26, 2019
* Refactor: renable web link in emails
* Refactor: clean up email web view
* Bug: webview should support lead id
* Refactor: update content page nav with new ux
* Refactor: initial component for NPS
* Refactor: clean up some responsive design
* Refactor: remove unused property

## December 24, 2019
* Bug: incorrectly check for null dsid
* Refactor: add support for skip take in contact document
* Refactor: mege ui into contact bundle
* Branch: initial change to support datatable in contacts ux
* Refactor: updates for contact search

## December 23, 2019
* Refactor: move search into apis
* Refactor: update contact document for new fields
* Refactor: add email dashboard
* Refactor: update references for sources
* Bug: trim items before inserting into index
* Refactor: create segment buttons on email clicks and opens
* Refactor: optimize for search ux

## December 20, 2019
* Refactor: add asset preferences for email
* Bug: querystring collection key can be null
* Refactor: start search page
* Refactor: add support for email data science
* Refactor: update search to support email metrics

## December 19, 2019
* Refactor: move search code from job into searchutil
* Bug: Segment pulling back results because field is null
* Bug: Milennial spelling

## December 18, 2019
* Refactor: update contact ux
* Refactor: ux and grammar updates
* Refactor: remove campaigns partial
* Refactor: contacts to move to api
* Revert: only pull in Active accounts for segments
* Refactor: add skeleton ux and convert segments
* Bug: hide skeleton
## December 17, 2019
* Bug: When everyone is selected in scheduler remove other segments
* Bug: ensure everyone is set if no segments selected
* Refactor: Add header to top of test emails that identify it as a test email
* Bug: limit max number of segments for message to 5
* Refactor: tune up campaign detail

## December 16, 2019
* Refactor: updates for filtered leads count
* Bug: convert contact change status to api
* Refactor: api for campaign recipient count
* Refactor: return stats for include exclude lists
* Refactor: convert to serialized dictionary
* Refactor: update scheduler to show approximate counts
* Bug: reference to save contact
* Refactor: change how timezone displayed in scheduler
* Refactor: schedule shows approximate recipients
* Refactor: add caching for Get Leads Stats

## December 13, 2019
* Bug: cookie secure interfering with path
* Bug: missed clone check
* Bug: don't load stats for invalid campaign id
* Refactor: lookup geocode for ip address
* Refactor: use token for ipinfo

## December 12, 2019
* Refactor: add issubaccount
* Refactor: clean up users warnings
* Refactor: start updates for admin panels
* Refactor: warnings for twilio not enabled
* Bug: email templates component can be null
* Refactor: use history cookie for better in-app nav
* Refactor: add support to clean templating strings
* Bug: tasks api call typo
* Refactor: add support for task type lead

## December 11, 2019
* Refactor: update to scheduler ux to handle overflow
* Refactor: updates for unsaved changes
* Refactor: rename ProcessRequest to ProcessReply
* Bug: fix user sort order

## December 10, 2019
* Bug: text color cannot be set by grapesjs trait
* Refactor: set grapejs color palette
* Refactor: remove link color from asset preferences
* Bug: link tracking bad javascript null check
* Refactor: copy url for content pages
* Bug: set settings to false for link tracking
* Bug: Push reports had bad links
* Refactor: text message replies
* Refactor: updates for text message reply view
* Refactor: add support for sms menus

## December 9, 2019
* Bug: add Remove stop word to text message opt out
* Bug: use dateoffset for reports
* Refactor: better handling of stop words and phrases
* Bug: if vs while for reading from database
* Refactor: add support for textmessagereply
* Refactor: formatting updates for email spools
* Refactor: text message reply model

## December 8, 2019
* Refactor: include segment name in export email notification
* Bug: handle text message credit based on number of segments
* Bug: set body margin to 0 on email preview html page
* Refactor: update email designer components for styles
* Refactor: log text message replies
* Bug: alignment and padding
* Bug: email designer bugs and layout

## December 6, 2019
* Bug: dates need to offset for sql query utc
* Bug: ready to send offset error
* Refactor: update scheduler to support editing
* Refactor: schedul api 
* Bug: push api included id

## December 5, 2019
* Refactor: updates to content page for build warnings
* Refactor: delete queue item before processing to guarantee not delivered more than once
* Refactor: remove drop down style on tasks

## December 4, 2019
* Refactor: asset preferences
* Refactor: audience dashboard
* Refactor: scheduled messages compiler warnings
* Refactor: audience report
* Refactor: notifications
* Bug: dequeue to 20 minutes
* Refactor: add asset preferences
* Refactor: exception handling for notifications
* Bug: updated async method for preferences
* Refactor: email designer support asset preferences
* Bug: Stretched image in messages for whitelabel
* Bug: remove float style option from email button
* Bug: set text color from asset preferences
* Refactor: copy asset preferences for sub accounts

## December 3, 2019
* Refactor: White label no reply
* Refactor: normalize notifications
* Refactor: audience reports
* Bug: ignore any age over 100 or under 18
* Bug: age reports should only use active contacts
* Refactor: change generation not set text

## December 2, 2019
* Refactor: run rebuild segments every 15 min
* Bug: slug in content pages should be set to empty when cloned
* Refactor: update 150 segments per-update
* Refator: remove archive from retargeting
* Refactor: add paused to web form
* Refactor: web form ux
* Refactor: set views to full width
* Refactor: update ux menus for retargeting
* Refactor: email status ux and add paused
* Bug: don't show campaign selector if campaign id > 0
* Bug: issue with space bar in email and page editors

## December 1, 2019
* Refactor: style and mobile updates
* Refactor: update segment update logic