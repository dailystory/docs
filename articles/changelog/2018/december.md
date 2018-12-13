{
	title: 'December 2018 Product Update',
	description: 'Product Updates for December 2018'
}
# DailyStory Product Updates for December 2018
## December 13, 2018
* Bug: advanced search may contain && which caused errors
* Bug: remove leads should reset lead table UX
* Bug: push bindings tool was not using index for display
* Refactor: move register device logic into PushNotifications
* Bug: segments to update filter
* Refactor: handle remove segement from campaign
* Refactor: RegisterDeviceAsync in Push Notifications

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