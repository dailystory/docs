---
layout: _ArticleLayout
title: July 2017 Product Update
description: Product Updates for July 2017
---
#July 28, 2017

* Fixed timezone bug in users

#July 27, 2017

* Added auto-resizing for tenant logo
* Addes support for copy/paste upload for images in emails, email templates, pages, and page templates
* Added BodyNoTemplate for email editing experience when working with templates
* Updated test lead for documentation
* Fixed typo in notification email
* Updated image store to add additional capabilities
* Better handling for webhooks
* Another fix for EmailWorkflowRule to handle am/pm changes

#July 26, 2017

* Updated popup editor with new close/cancel options
* Changed Tenant Timeoneoffset to store timezone string for dst calculations
* Compressed CSS files
* Updated/added more unit tests
* Better datetime handling in date formatters
* Added DST calculations to timezone lookup tables
* Added option in exit intent to hide close/cancel button
* Changes to EmailWorkflowRules to handle DST

#July 25, 2017

* Added QUnit tests for DailyStory javascript libraries
* Refactored page loading and progress loading to display messages
* Refactored controllers to pass data center via tenant directly
* Refactored naming on misc async methods
* Added better exception handling to forgot password
* Updated Ds script to continue to improve page path analysis
* Added easy close option and delete state cookie to popup
* Updated Contact and Lead tables to use Friendly Date formatter
* Fixed bug in login for forgot password (wrong url in error message)
* Converted trial to use new progress on/off for long running data creation process
* Fixed bug in license banner path
* Updated unit tests
* Moved all jobs to use built in Azure publishing
* Fixed bugs in cron for jobs that was causing over execution
* Updates to campaign workflows to ensure single lead goes through a workflow
* Moved trial clean up logic into Trial class
* Began moving logic out of search job and into respective object classes
* Refactored TrackingListStats to no longer be a per-tenant loop job
* Added search connection string management to connection provider
* Refactored lead based on tests
* Added IsExpired check to license
* Added logic to lookup tables based on tests
* Refactored CampaignRuleSet based on common patterns
* Updated Trial class to handle creation of trial data set
* Refactored User based on test cases
* Refactored CampaignWorkflow based on test cases

#July 20, 2017

* Update LeadStats job to better handle last seen and first seen
* Update ProcessLeadQueue to ignore duplicates
* Update Common to use ArgumentException
* Update Contact to use upper case on words
* Refactored ContentPages
* Added document provider to connection provider
* Updated data import to not import duplicate leads
* Updated Email to use ArgumentException
* Updated Lead QueueItem for duplicate handling
* Updated integration tests for refactoring
* Updated Lead to better handle data integrity on save
* Refactor LinkTracking
* Refactor RetargetPixel
* Added caching support to conversion rate report
* Refactored ContactDocument
* Added Async operation on Get Tenant
* Added Trial class for populating new trials with sample data
* Updated trigger web job to reflect moves in jobs
* Added support for javascript tests
* Added upload image support for email
* Refactored controllers based on design changes
* Updated DS script to better handle paths and urls in pages check
* Removed event from campaigns temporarily
* Fixed bug in FriendlyDateTime
* Fixed bug in LInkTracking javascript campaign picker

#July 18, 2017

* Added support for image upload in email editor
* Refactor Campaign class based on unit tests
* Update to most recent version of Tiny MCE
* Fixed conflicting column bug with Contacts
* Update to Contact class to use ContactStatus
* Internal clean-up / method renaming
* Added caching to reports to improve performance
* Added server side validation check for urls
* Update image store to handle support for folders
* Refactored webhooks based on tests
* Updated Jobs to use dedicated server to prevent blue/green name issues
* Updated CampaignWorkflow to use enum values instead of hardcoded ints
* 

#July 17, 2017

* Updated trial workflow to auto-sign in users
* Update Messages controller to handle exceptions
* Cleaned up trial process in Home Controller
* Refactored email controller and class to better handle errors
* Refactored Contact based on new test cases
* Better error message on Email API
* Added additional unit tests
* More error handling based on unit tests
* Added exception handling for Data Provider 
* Refactored lead to use date last contacted for date lookups
* Refactored Contact Document based on unit tests
* Added more exception handling to Tenant
* Created Trial class to contain trial logic for testing
* Updates to validation class

#July 15, 2017

* Completed refactoring of email and email templates and associated tests
* Added new license exception class
* Completed refactoring of notification and associated tests
* Converted from return types to exceptions
* Began standardizing cache key names
* Removed non-async methods from email providers

#July 13, 2017

* Added custom error handlers for API
* Converted store methods to use async as part of test pass
* Updated AuthorizationBaseController for APIs
* Finalized Email REST API for sending
* Added DotNotContact method
* Added Error Controller for handling errors better
* Removing use of LightningContext.User from generic methods in Common class
* Removed track clicks toggle (always on)
* Added 404 handler for non-customers
* Added more unit tests for API coverage
* Fixed bug in MailgunSync
* Added status code to ApiResponse class to enable developers to better handle conditions
* Additional updates/improvements to common class

#July 11, 2017

* Added an additional 148 unit tests over the past 2 weeks.
* Small change to Common formatting method to use Utc naming vs. Gmt
* Removed login with token for trial process
* Cleaned up trial process in preparation for auto-sign in from Google
* Refactored CampaignWorkflow job to enable easier testing moved logic to CampaignWorkflow class
* Converted rules to Async
* Fixed cache key conflict with Data Manager
* Added error checks to Common library
* Clean up / refactor to email and email templates
* Refactor lead and convert to MemoryCache
* Added new exception types to lightning exception
* Refactored lookup on timezone table to handle default timezone from Tenant
* Added dsid property to LeadStats and refactored Url lookups to improve perf.
* Updates to RulesEngine basd on tests and added support for string comparision that doesn't care about case
* More fixes to EmailWorkflow rule