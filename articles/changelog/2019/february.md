{
	title: 'February 2019 Product Update',
	description: 'Product Updates for February 2019'
}
# DailyStory Product Updates for February 2019
## February 28, 2019
* Refactor: support birth date and generation
* Refactor: common calculate to generation and birthday
* Refactor: semi-hack to fix sparkline load filcker
* Refactor: control extended fields for export
* Bug: email delivery report email id bug

## February 27, 2019
* Bug: date time calculated incorrectly
* Refactor: remove organization from graph 
* Refactor: select2 styles
* Bug: set view in browser toggle in save
* Refactor: clean up advanced settings
* Refactor: inline material checkbox in modal
* Refactor: capture address and phone in tenant
* Refactor: include export custom field
* Refactor: better exception handling

## February 26, 2019
* Refactor: move select2 css out of tasks
* Refactor: API emails to get directly from form post
* Refactor: plain text form
* Refactor: add send email to contact from index
* Refactor: add merge plain text body
* Refactor: re-enable refresh campaigns
* Bug: preview url for file assets

## February 25, 2019
* Refactor: standardize drop down toggle UX
* Refactor: update file icons
* Refactor: toolbar for files

## February 22, 2019
* Refactor: add file pickers into nav; copy url clipboard

## February 21, 2019
* Refactor: can't change data type or remove index from indexed custom property
* Refactor: contacts table view

## February 20, 2019
* Refactor: updated graph fields for add/remove and unit tests
* Refactor: [Mindbody] better date sync per client and add additional unit tests
* Refactor: more detailed exceptions for opt-outs
* Refactor: finalize behaviors on custom fields

## February 18, 2019
* Bug: handling nulls for UDF fields
* Refactor: add separate sync datetime stampe for Mindbody
* Refactor: refresh campaigns
* Refactor: edit support for graph and picklists

## February 17, 2019
* Refactor: add better save ux
* Bug: remove iframe tags from email html
* Bug: search filter should honor timezone offsets

## February 15, 2019
* Refactor: performance improvements to AddSegmentToCampaign
* Refactor: set date last indexed to null on contact update
* Refactor: add save batch to lead
* Refactor: display not ready for email delivery report
* Refactor: don't look up trials or demo accounts in prod

## February 14, 2019
* Refactor: meeting events
* Refactor: performance enhancements for segments
* Add: segments REST api
* Refactor: scheduler excluded segments don't need to be part of campaign
* Refactor: add IsReportReady to email report
* Revert: add set property back to fullname

## February 13, 2019
* Refactor: add warning when modifying segments of a campaign that has workflow
* Refactor: move workflow logic into core
* Revert: process set isindexed
* Refactor: add api to kill queue items
* Refactor: begin use of return struct for test validation
* Refactor: move process workflows into core
* Refactor: ensure tasks are dequeued once

## Feburary 12, 2019
* Bug: contact fullname wasn't being refreshed correctly
* Refactor: return email struct to verify pesonalization in test
* Refactor: use email struct in handlebars compilation
* Refactor: add last visit date to mindbody installer
* Refactor: lead queue item will only enqueue leads to active campaigns
* Refactor: Lead save set tenant; check for empty dsid; validate campaign is active
* Refactor: add email struct and workflow exception
* Bug: if wait until is > 1 day old throw exception to invalidate the lead
* Refactor: trial to use lead save with tenant
* Refactor: lead automation to use tenant in save
* Refactor: notifications to use updated merge html

## February 11, 2019
* Bug: segment save issue with recent refactor tenantid not set
* Refactor: add campaign refresh logic
* Refactor: add delay in refresh campaigns; better exception messages
* Refactor: add support for RefreshCampaigns to tasks
* Refactor: add support for excludes in scheduled messages
* Refactor: handle segments of 0 length
* Bug: validate campaign is active prior to sending

## February 9, 2019
* Refactor: add support for excluding segments and refactor campaign send
* Refactor: update scheduler to modal

## February 8, 2019
* Refactor: move azure functions to separate project
* Bug: eliminate uncessary database call
* Refactor: add pick list field to graph
* Refactor: performance enhancements to segments
* Bug: premailer threw unhandled exception for bad css url

## February 6, 2019
* Bug: magic form please wait not turning off on create
* Refactor: mindbody license check update
* Refactor: add browser check on home
* Refactor: update media calendar
* Bug: move browser checks to separate js file due to IE issues
* Refactor: MINDBODY better api management and capture last visit date
* Refactor: update webforms for new ux
* Refactor: change webforms get to be more consistent
* Refactor: pick list custom fields

## February 5, 2019
* Refactor: add link for create when there are no results
* Bug: fix background color of default popup
* Refactor: add online help links to sms
* Refactor: job manager insert and null checks
* Refactor: update search to not use date_last_indexed
* Refactor: move get contacts to update to contact document
* Refactor: check if date is in the future
* Refactor: add DateTime comparison to ifEqual
* Bug: handle enumeration collision in set extended properties
* Bug: handle invalid phone number

## February 4, 2019
* Refactor: pick image dimensions and description
* Refactor: add upload support to file picker
* Bug: modal button styles to footer only
* Refactor: update tasks to use file picker
* Refactor: add file name to breadcrumbs and reset title
* Refactor: more gracefully handle errors in debug mode for integrations

## February 3, 2019
* Refator: change user agent header for opengraph requests
* Refactor: add clear already received
* Refactor: delete events if they object was deleted
* Bug: handle bars compile with null name
* Bug: lead should be able to receive the email more than once
* Bug: preview url could double entry
* Refactor: close modal and updated preview url

## February 2, 2019
* Feature: file manager picker initial check-in
* Refactor: pick and list files for file picker
* Refactor: add dimensions and image preview

## February 1, 2019
* Bug: select all in contacts not calculating correctly
* Bug: remove prevent default
* Bug: test segment button added extra s=