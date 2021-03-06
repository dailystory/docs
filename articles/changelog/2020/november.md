# DailyStory Product Updates for November 2020
## November 30, 2020
* Contact Search not returning correct results for Custom Field: Coterie/Role Field
* Progression on support for accounts

## November 27, 2020
* Validate from address matching to allowed sender when creating an email
* bugs with account saving
* edit create for account

## November 25, 2020
* Add support for create, edit and view accounts

## November 24, 2020
* Automation fix for handling no only condition in some cases
* Add lead to campaign when lead exists but is deleted
* Lead campaign status should be reindexed

## November 23, 2020
* Sort order on tasks
* temporary fix for setting bool values when editing contacts

## November 21, 2020
* Automation condition "Is in segment" should allow multiple segments to be selected
* Convert elipse drop downs to boostrap 4

## November 20, 2020
* Style updates
* Bug with file / folder load order in file picker'

## November 19, 2020
* Only drag using handle

## November 18, 2020
* Add link on Failed SMS report page to article with violation codes
* Ensure a valid email can't be swapped to a @example.com email
* Opt out report needs to pull +1 day in order to pull data in for current date
* Support folders for organizing campaigns

## November 17, 2020
* Updates to RSS trigger logic
* Azure function to trigger RSS changes
* Set font sizes and default back to Helvetica

## November 16, 2020
* Add caching for favorites look ups
* Retry on sql timeout exception

## November 12, 2020
* Update old activities to render correctly in activity log
* UX improvement to lead activity

## November 11, 2020
* Helper in asset preferences to format email address
* Track clicks and opens by domain for emails
* Delivered should be clickable from email summary report
* Update texts and push notifications to use tenant's timezone for date logging
* Bug with frequency selection in rss updates
* Support for TriggerWhenRssUpdatedAsync
* Handle SQL timeout exceptiosn and cool down

## November 10, 2020
* Bug with reindex partial never ending loop
* Partial reindex of status was int should be string
* Filter get contact by status
* improvements to auto generated plaintext

## November 9, 2020
* Reorg RssEmailUtility into RssHelper
* allow block to specify which children are allowed to snap
* Add TriggerWhenRssUpdated
* Bug with remove from campaign action

## November 7, 2020
* Add RSS trigger block
* Allow automation block to be set as disabled

## November 6, 2020
* Convert click report to use datatable and include URLs
* Add support for AMP emails
* Tracking links need to set campaign id
* Set utm_content to id of email in email redirects
* Add bulk add/remove tags from contacts
* add additional activity types such as send sms

## November 5, 2020
* Opt out reports needs to include contact details
* Allow magic form to auto-choose form with most fields
* optimize TZ lookup to skip exceptions
* Don't auto create plaintext for email
* Better routine for generating plaintext without requiring additional html parsing
* more css/html optimization
* handle nulls in graph field exports
* Updates for email opt out detail by email id
* Allow exports for opt out by email id
* handle neverbounce exceptions for insufficient credits
* Show error message when invitation code is invalid

## November 4, 2020
* Column sort order for last modified on leads is not returning correctly
* Iteration on Send a reply on top of an existing email design widget

## November 3, 2020
* Replace Poshy tooltip with Tooltip.js
* More style clean up
* Timeout issue on contact activity
* Graph field need to check for null or empty pick list
* Email Bounced List EXPORT report not working
* update to latest version of jquery
* update to latest bootstrap

## November 2, 2020
* Clean up and reorganize css
* Specify the lead origin when lead's created through automation
* Move images to CDN
* Consolidate lighthouse script
* contact log post method wasn't sending back new entry id

## November 1, 2020
* Convert contact activity to contact log and to javascript
* Convert autopilot action to use contact log
* Bug with leads that are restarted in workflow prevent new leads from getting processed
* Define a user id for log entries written by automation
* Update contact preferences to use ContactLog
* Stacked images in email should be display block if width is 100%
* Set styles for designer emails
* Don't display age information if no age data in audience report
* Remove unused CSS and clean up old files
