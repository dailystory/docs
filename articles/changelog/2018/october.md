{
	title: 'October 2018 Product Update',
	description: 'Product Updates for October 2018'
}
# DailyStory Product Updates for October 2018
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
