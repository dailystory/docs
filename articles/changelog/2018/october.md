{
	title: 'October 2018 Product Update',
	description: 'Product Updates for October 2018'
}
# DailyStory Product Updates for October 2018
## October 31, 2018
* Feature: change password
* Refactor: updates for unit tests

## October 27, 2018
* Refactor: better logging during bulk import
* Refactor: unit test updates

## October 25, 2018
* Refactor: typos and other misc
* Refactor: update titles

## October 23, 2018
* Bug: whitelabel error handling messages
* Bug: get any campaign
* Bug: White label some admin screens

## October 22, 2018
* Bug: email missing from add to segment queue
* Feature: tasks add segment to campaign and all all contacts
* Refactor: API ContactList > Segment and use tasks for background processing
* Bug: select all in leads not working

## October 21, 2018
* Bug: phone number could throw exceptions
* Refactor: add dictionary parsers for filters
* Feature: inline css in emails
* Refactor: check if campaign exists by name; used in clone
* Refactor: better filtering for segments
* Bug: secondary button style bug
* Bug: ApiName not persisted

## October 18, 2018
* Remove: returning contacts report is redundant
* Refactor: DailyDigest to use search
* Refactor: Segments controller returns Any

## October 17, 2018
* Refactor: fix build warnings
* Refactor: improve exception handling for tenant not found
* Bug: schedule to send text shown when nothing scheduled
* Bug: update segment date_last_modified to occur in the past to allow for update
* Bug: btn-secondary doesn't render correctly
* Refactor: refactor dynamic segment refresh
* Refactor: handle errors in search for dynamic segments
* Feature: initial check-in of deep clone campaign

## October 16, 2018
* Feature: added ProcessTaskQueue
* Bug: LastVisitDate can sometimes be null for Telligent integration
* Refactor: better api counting for mindbody
* Feature: Azure function to add task for rebuilding dynamic segment
* Bug: handle DateLastSeen min/max values for SQL
* Bug: handle empty title in content pages and properly set status
* Refactor: ContactList to Segment methods
* Feature: Tasks
* Feature: add support for trigger web job for task queue
* Refactor: support N days back for search queries
* Bug: contacts in dynamic segment cannot be removed

## October 15, 2018
* Refactor: set date last seen in contact save
* Refactor: update telligent installer
* Refactor: better error message for Salesforce sync
* Bug: MindBody activation url needed to urlencode activation code
* Bug: MindBody modal referenced bad image path
* Refactor: consistent page titles
* Refactor: removed updated column from contacts tables
* Refactor: handle view cases for home page
* Refactor: Improvements to contact header

## October 14, 2018
* Feature: auto-install contact field properties for integrations
* Refactor: Graph Field
* Bug: optin mindbody on PromotionalEmailOptin
* Refactor: update contacts to support array of user defined array
* Refactor: split populate contact document function
* Refactor: add auto install option for MindBody and Telligent
* Refactor: update contact detail to support array of udf strings

## October 13, 2018
* Refactor: scheduled message and add send method
* Refactor: roles update and enable in side bar

## October 11, 2018
* Bug: handle exceptions in SF lead creation edge case

## October 10, 2018
* Refactor: Add auto-save to emails
* Bug: MindBody handle addresses and PostalCode
* Refactor: add support to campaign workflows job to run campaign schedules
* Refactor: add support to MindBody to get activation code for siteid
* Refactor: add support for event logging to Telligent plugin

## October 8, 2018
* Bug: MindBody integration needs to sync on ID not UniqueId
* Bug: Remove binaries from Telligent Sync
* Feature: sync additional user fields for telligent
* Bug: cookie property from plugin not set correctly
* Bug: scheduled message id had typo in evaluation
* Feature: scheduled email sends
* Refactor: added option to filter List on Leads by campaign
* Refactor: Remove old MindBody files add integration settings
* Refactor: Delete integration settings option
* Feature: add telligent integration settings

## October 6, 2018
* Refactor: Safety check to prevent leads from receiving the same email more than once
* Feature: add schedule message
* Refactor: css updates for date time picker z-index
* Refactor: css updates for input group buttons
* Bug: set stream reader position
* Feature: add api for getting email's schedules
* Refactor: update tools
* Feature: updates for new email send features
* Bug: lead should filter extended properties shown in UX

## October 5, 2018
* Refactor: Contact Device
* Refactor: update modal header style
* Feature: tools - send push, get bindings
* Feature: support for confetti
* Refactor: send now option for email
* Refactor: register push device ids

## October 4, 2018
* Refactor: Address lookups using Google Location API need to cache in storage to prevent API over use
* Refactor Store device id when a user registers a device for push.

## October 3, 2018
* Bug: api global errors should return a http 400
* UX: hide company field if it is not populated
* Refactor: add phone number formatter
* Refactor: contact and lead activity for new contact detail view

## October 2, 2018
* Feature: add support for Telligent as integration type
* Bug: size thumbnail to max 80 width
* Bug: Contact search should work with return key

## October 1, 2018
* Feature: Add MindBody to integrations
* Refactor: add support for setting api name in graph field
