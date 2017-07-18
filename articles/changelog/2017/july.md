---
layout: _ArticleLayout
title: July 2017 Product Update
description: Product Updates for July 2017
---
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