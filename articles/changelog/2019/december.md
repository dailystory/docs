{
	title: 'December 2019 Product Update',
	description: 'Product Updates for December 2019'
}
# DailyStory Product Updates for December 2019
## December 12, 2019
* Refactor: add issubaccount
* Refactor: clean up users warnings
* Refactor: start updates for admin panels
* Refactor: warnings for twilio not enabled
* Bug: email templates component can be null
* Refactor: use history cookie for better in-app nav
* Refactor: add support to clean templating strings

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