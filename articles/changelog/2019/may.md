{
	title: 'May 2019 Product Update',
	description: 'Product Updates for May 2019'
}
# DailyStory Product Updates for May 2019
## May 30, 2019
* Refactor: content page editor
* Add: api for fetching web forms
* Refactor: update controller for unit test
* Refactor: add support for Twilio webhook url in admin ux
* Refactor: support preview url on content pages
* Bug: can't using LightningContext in components
* Refactor: use please wait screens for saving
* Refactor: return tenant information with Twilio webhook api
* Refactor: clean up page components
* Refactor: update dynamically from rte

## May 29, 2019
* Refactor: handle null condition in web tracking callback
* Bug: incorrectly marking failed SMS sends as optout
* Refactor: separate out count of emails to send
* Bug: force removal from cache on preview for links
* Refactor: support for Twilio voice and copilot
* Refactor: set a default value of 0
* Bug: api name on graph field is immutable

## May 28, 2019
* Refactor: improve handling of paths through tracking logic
* Remove: unused ds css and js
* Remove: dead code
* Bug: select not properly wrapped in selector
* Refactor: updates for redirect hash
* Bug: fix bug in email url rewriting that could result in errors

## May 25, 2019
* Refactor: add header only if a value is found
* Refactor: add assembly information to jobs
* Refactor: better exception handling for missing url
* Refactor: handle api params as method params on controller

## May 24, 2019
* Bug: throw exception if segment has greater than 100K members
* Refactor: shortcut dynamic segment logic if no members
* Refactor: move string array skip to common
* Bug: no longer need total_members and optimize cache of list
* Refactor: don't cache list of segments for view
* Refactor: merge in new sent from options
* Bug: save new email shouldn't validate sentto options

## May 23, 2019
* Refactor: add replyto header for email
* Refactor: skip items for webforms
* Bug: handle form type for data entry
* Refactor: better controller unit testing web forms
* Refactor: handle replyto in web ux
* Refactor: commercial version of font awesome
* Refactor: change how whitelabel logos are managed and load from CDN

## May 21, 2019
* Refactor: support better import to segment options
* Refactor: remove camapign and add segmentid
* Refactor: updates to support segments lookup
* Refactor: search filter should ignore import_segmentid
* Refactor: allow segment lookup by segment name
* Refactor: log version and data center in jobs

## May 20, 2019
* Refactor: update for managing segments during import

## May 17, 2019
* Refactor: standardize css for select bar
* Refactor: campaign api for adding leads by dsid
* Remove: old add lead 
* Refactor: update UX for new add campaign/segment behavior
* Refactor: batch add leads by dsid
* Refactor: save batch returns array of lead ids
* Bug: segment names should be unique

## May 16, 2019
* Bug: should be able to add to imported segments
* Refactor: cache optout report
* Refactor: Campaign picker should be a modal with search
* Refactor: return lead from controller api

## May 14, 2019
* Bug: CDN url redirecting to non-https
* Bug: bad query for opt out report

## May 13, 2019
* Bug: rot13 decoder needs to handle http urls
* Refactor: add validation to validate send time
* Refactor: handle license exceptions more gracefully

## May 10, 2019
* Refactor: add caching for clients lookup in Mindbody
* Refactor: handle email format validation issues in NeverBounce

## May 9, 2019
* Bug: handle invalid email address
* Refactor: updates for better versioning
* Refactor: isEmailEnabled and Email verification
* Refactor: if not allow from cache, flush cache

## May 8, 2019
* Refactor: cache the license check
* Refactor: merge license warning css
* Refactor: merge license callback into ux common
* Refactor: add sms credit check to create edit screen
* Bug: name was not shown in quick send

## May 6, 2019
* Bug: update test for changing synced email
* Refactor: process status queue with send loop
* Refactor: licensing warnings and errors

## May 3, 2019
* Bug: bad link to failed SMS
* Bug: missing pages for failed sms
* Refactor: add exception logging for sms and email apis
* Bug: trim could check on null string
* Bug: ensure that a dsid is only updated once in a bulk upsert
* Bug: handle exceptions with Google API
* Refactor: add support for postal code to contact search
* Bug: handle issues with text message contents that are too long
* Refactor: add support in ux for postal code