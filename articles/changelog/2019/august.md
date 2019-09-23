{
	title: 'August 2019 Product Update',
	description: 'Product Updates for August 2019'
}
# DailyStory Product Updates for August 2019
## August 30, 2019
* Bug: content gallery not bringing over email css
* Bug: remove empty MBO services
* Bug: check max length on city field
* Bug: include css in email preview in gallery
* Refactor: add layout container for email designer
* Refactor: add support for videos component

## August 29, 2019
* Refactor: [Email] add preview and post for designer
* Refactor: [Email] designer updates to default editable components
* Refactor: [Email] add preview option
* Refactor: [Gallery] updates to email preview
* Refactor: [Email designer] updates to better handle css, preview and design changes
* Refactor: add year to templating engine
* Bug: handle nulls in templating for @ entries
* Refactor: add push sent report
* Refactor: mbo only available for commercial editions
* Refactor: [Push] add filter for sent only
* Refactor: log bad dsids
* Refactor: handle css that is inline in the email
* Bug: handle links in designer html body

## August 28, 2019
* Refactor: reorganize email designer components; inline styles
* Refactor: move load into script for email designer
* Bug: reset tabs for page designer
* Bug: show no preview when not active for landing pages
* Refactor: email designer updates
* Bug: images could get overridden with no image
* Refactor: add support for app icons in designer
* Bug: divider is a Layout not content section

## August 27, 2019
* Refactor: [Bug] better handle hide RTE in grapes
* Refactor: [Email designer] updates and changes
* Refactor: add undo redo and preview
* Refactor: [page designer] change how rte is handled to allow inline edit

## August 26, 2019
* Refactor: add support for push notification reports
* Bug: [Popup] no copy option
* Bug: [Popup] url should change on save
* Bug: status message remove instead of hide
* Refactor: remove old files add image for designer
* Refactor: better UX for item cannot be added and track state
* Remove: campaign reports - move to new repor

## August 23, 2019
* Refactor: show username and last login in preferences
* Bug: [link tracking] copy link broken
* Bug: [Popup] save covers save button
* Bug: [Popup] popup should use CDN for images
* Refactor: [File Manager] simplify CDN path logic
* Refactor: change breadcrumb nav to go to campaign vs. filtered search
* Bug: [Content Page] asks for leave site when no changes have been made

## August 22, 2019
* Bug: [MindBody] remove services if no longer valid
* Refactor: [Popup] allow forcing a popup to be shown via js api
* Bug: first item in segment could get removed if not added first
* Bug: Css missing for enabling edit of head section
* Bug: head changes not saved

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