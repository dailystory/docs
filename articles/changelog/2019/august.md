{
	title: 'August 2019 Product Update',
	description: 'Product Updates for August 2019'
}
# DailyStory Product Updates for August 2019
## August 20, 2019
* Bug: [Mindbody] update GetClientService to include CrossRegionalLookup
* Refactor: [D37] individual donor lookup
* Refactor: [D37] GetDonorInfoAsync to GetDonorsAsync
* Refactor: Professional default selected license
* Bug: javascript referring to same variable
* Bug: [MindBody] force sync wasn't implemented
* Refactor: [Mindbody] handle cross-regional users

## August 19, 2019
* Refactor: [Tracking Links] add license checks to handle limits
* Bug: handle test dsids in email click open queue and dsid validation

## August 16, 2019
* Refactor: [Cms] don't allow auto-redirects on expired or trials

## August 15, 2019
* Bug: [Lead] missing javascript and removed back button
* Bug: [TextMessage] remove delay
* Refactor: clean up copy and remove old references

## August 13, 2019 
* Refactor: [Store] purchase single item invoice and text message credits
* Refactor: [Text Message] move update credits into this class
* Refactor: [Store controller] initial check in
* Refactor: Update usage report to include purchase text message credits
* Refactor: [Text Messages] finalize support for purchase credit
* Bug: [TextMessage] PurchasedTextMessages can't be interal
* Refactor: [Login] redirect urls to switch to a tenant
* Refactor: [Notifications] use new lead tenant links
* Bug: [License] check for text messages was done incorrectly
* Bug: [Mindbody] don't display auth key if license prevents usage

## August 12, 2019
* Bug: [TextMessage] invalid argument check
* Refactor: [PushNotification] handle unsent a reorg code

## August 11, 2019
* Refactor: credit clarification for text messages
* Refactor: [Text Messages] add support for text message credits and checks

## August 9, 2019
* Bug: push disabled by default; enabled when a device id is registered
* Refactor: update D37 build package
* Bug: internal set prevents serialization; force license checks for free, trial, etc.
* Bug: [Popup] Report shows no popups when should say no leads
* Bug: [Search] ranged search, such as dateTo and dateFrom should not be case sensitive
* Feature: [Email Report] add email id to email summary report output
* Bug: [Mindbody] Require commercial license to add MBO integration
* Refactor: single method for checking if restricted class of service
* Refactor: text updates in admin

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