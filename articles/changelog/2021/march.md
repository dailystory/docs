# DailyStory Product Updates for March 2021
## March 12, 2021
* New popups are paused by default
* Fix some save issues in popup
* Updates to contact preference logging with auditing
* Updates to return leads in progress for autopilot
* Bug with sms reporting
* Bug an item with the same key has already been added

## March 11, 2021
* Skip null activities
* Updates for responsive
* Exception handling when trying to convert an extended property for export
* Optimize records returned in delivery report
* Leads in workflow should return full list
* Cache workflow leads for reports
* Check for dsid instead of lead id for submits
* Update conditions on form submits

## March 10, 2021
* Bug with submitted web form automation trigger
* Support segment cloning
* Updates to cache logic for Redis
* Refactor how unsubscribes in emails get logged
* Ensure a contact look up happens if not found in cache
* Convert email opt out reports to not use ds_email_log
* Reload the email prior to saving

## March 9, 2021
* Text message MMS image check should be 640 not 600
* Updates for allow local cache
* Update to tenant to handle Account Owner

## March 8, 2021
* Remove reindexing from functions
* Clean up salesforce sync
* Helper method to update string if value has changed
* Bug with new tenant creation script
* Contacts support bulk edit mode

## March 7, 2021
* Refactor email activity item
* Refactor tenant to use Redis cache
* Refactor Text Message activity for performance and batch updating
* Twilio throws messagenotfound exception
* Ensure exception logging is string bounds checked
* Bug with Tenant switching

## March 6, 2021
* Longer cache duration for sms logs
* Use Redis for DataManager caching
* Undo changes to use Redis for contact avatar

## March 5, 2021
* MMS size check and impact to deliverability score
* Allow send single for email
* Add new cache layer for Redis
* Update segments and tenant to use redis
* Update SmsActivityItem to use Redis
* Refactor contact and lead for redis caching
* Refactor campaign and segments for Redis caching
* Refactor how avatar URL lookups are handled
* Use Redis for contact lookup
* Leads in inactive campaigns should not be included
* Sort segments and campaigns in contact detail
* Sort tags alpha on contact

## March 4, 2021
* Lead id not properly set for popover in campaign more than once
* Contacts that come through the lead queue and are marked as spam
* Link click condition needs to handle first url in list as no change event is fired
* Better css for automation designer
* Add segments to campaign from segments list view

## March 3, 2021
* Azure functions need to run at 6am UTC to run at midnight
* Clicking favorite need to prevent default scroll
* Add padding to email subject in editor to prevent overflow

## March 2, 2021
* Reset designer pill tabs
* Performance improvement for license checks that are not needed
* Begin conversion to CosmosDb
* Date and time on activity feed is incorrect
* Ability to assign a task from within a contact record

## March 1, 2021
* Performance updates
* Templates not populating Template Gallery UX Page from "Template Gallery" link
* Handle sql deadlock retries
