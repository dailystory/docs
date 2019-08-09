{
	title: 'August 2019 Product Update',
	description: 'Product Updates for August 2019'
}
# DailyStory Product Updates for August 2019
## August 8, 2019
* Refactor: add hasown license for email and sms
* Bug: avatars for users that don't start with a letter breaks
* Bug: handle less than zero
* Bug: hide sms license detail if user has own license
* Bug: json formatting for licenses
* Bug: fix table report summary display with long name
* Bug: handle long breadcrumb text with elipses

## August 7, 2019 
* Refactor: change email task count
* Refactor: change method names and behavior for license refactor
* Bug: api key license check does not need to be async
* Refactor: reorg license class and methods
* Refactor: reorg LicenseCheck and methods
* Bug: user checks used campaigns

## August 6, 2019
* Refactor: mail spoolers for Mailgun
* Refactor: delivery queue for delivery status
* Refactor: simplify email jobs methods
* Bug: ensure data center is in the correct format for lookup
* Bug: inbound Twilio webhook url should always be available
* Bug: page create could get stuck on saving
* Bug: change email summary report to use offset for cache duration
* Bug: code / reason may not exceed length

## August 5, 2019
* Refactor: process email delivery separately
* Refactor: Add support for SendBulk
* Refactor: improve performance of email status queue
* Refactor: add support for update batch Email Activity

## August 3, 2019
* Bug: unsend text messages that fail to send

## August 1, 2019
* Bug: handle marking email as unsent for errors
* Bug: handle setting visit date for MBO customers that never visited
* Bug: bound check reason and code on email activity
* Refactor: convert to await when all on email tasks
* Refactor: initial support for mail spoolers
* Feature: initial checkin of mail spooler job
* Refactor: improve performance of email stat updates