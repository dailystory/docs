---
layout: _ArticleLayout
title: June 2017 Product Update
description: Product Updates for June 2017
---
#June 26, 2017

* Performance improvements to campaign workflows job
* Added option in Job Manager to control whether or not datetime is needed (reduce SQL per tenant)
* Update to RunCleanup job to execute every day at UTC 6a
* Moved SQL logic from run clean up to a stored procedure
* Update email integration interface to support general headers list
* Added Salesforce update to get opportunities
* Updated Account to use Table Storage for storing quality calculations
* Updated Achievements to remove sum of web achievements
* Updates to Contact to support Delete and Updates
* Refactor of Connectionprovider
* Added licensing check in email to ensure trials cannot exceed limitations
* Changed email template management to async loading
* Added list-unsubscribe header to emails
* Changed merge tags logic to be async and removed regex
* Refactor on Email Activity and changed to async
* Refactor lead activity for async
* Refactored Web Activity with performance improvements and async
* Removed Wait() operation on Lead
* Added duplicate logic check on Lead save vs as a job (performance improvement)
* Added support for emails per month license and to license check
* Refactored Lookup country to support reverse lookups by country name
* Fixed typo in LookupIndustry
* Added logic to timezone look up to return tenant default when lead doesn't have a timezone set
* Updated Notifications to use async
* Updated campage email report to return count in sparklines vs percentage delivered
* Updated Lead Summary Report to use async
* Fixed bugs in Exit Intent Report and simplified
* Performance improvements to Web Session Detail Report
* Added more debug logic to Campaign Rule
* Removed Email Replied from campaign rule selector
* Added Website engagement score to use Azure storage
* Added AccountDocument and ContactDocument for storage and management in Azure search
* Updates to initial tenant look up for datacenter connection string managment
* Updated pay per click sql and logic for async and performance improvements
* Added Trigger Web Jobs to enable remote triggering of web job via webhook
* Added timezone support to account
* Added Pipeline lookup for Campaign
* Initial check in for Email and Lead Reports controller
* Updated license usage report to refect email sent counts
* Removed sum of web views from web activity



#June 21, 2017

* Performance improvements and bug fixes to jobs
* Updates Update Leads to include a column to get a better index
* Removed duplicate lead check - too exensive. Instead checking for duplicates on insert
* Converted IP look up to run for all tenants in data center vs as a per-tenant job
* Updated account scoring to run a parallel thread for each tenant, may re-evaluate
* Fixed bug in job used to update Azure search to limit the number of records in each back to 100
* Removed duplicate entry to update web stats

#June 20, 2017

* Updates to Exit Intent report to simplify data returned and fixed a bug in date calculation
* Added support for unsubscribe to emails to force opt out on an account
* Trimmed back merge code to remove unncessary descriptions
* Removed LeadActivityReport from Lead Model, not sure why it got added
* Renamed Exit Intent CSV export file
* Converted LeadSummaryReport to use async
* Converted ActivityTimeLine to use async

# June 18, 2017

* Add API to account controller to return website engagement score
* Changed all emails to use async and added Email Model

# June 16, 2017

* Performance improvements to jobs to decrease SQL calls
* Added check to campaign workflow to skip campaigns that didn't have workflows
* Converted ProcessTriggerQueue to continuous program empties a queue
* Removed old files from ProcessWebLeads
* Changed sleep logic in WebTrackingQueue
* Fixed bug in Salesforce Sync and added support for updating opportunity values
* Initial checkin of Account Score job
* Updated UpdateSearch job to handle account and contact deletes to remove from index

# June 14, 2017

* Added UpdateSearch web job for updating Azure search with changes to Contacts and Accounts
* Updated all jobs to .NET 4.5.2
* Updated lightning.css to add css for account status
* Added support for create account flow
* Added API for account
* Updated contact controller to redirect to contact when search returns single result
* Added javascript file for updating account
* Removed requirement for Company name when creating a new contact
* Updated account detail to include website activity and stubs for account scores
* Fixed HTML bugs in campaign create/edit
* Changed accept / reject lead to use colored buttons to stand out more
* Added Cancel option to save buttons library

# June 11, 2017

* Move to .NET 4.5.2 and library upgrades
* Added support for Azure search in Accounts and Contacts
* Fixed bug in ContactController that was passing incorrect enum
* Added support to Contact and Account search to be intuitive/friendly UX
* Added jquery plugin to set cursor to end of selection on pre-filled textbox
* Added links to web activity
* Early modification to activity tracking for contact
* Stubbed in connection provider logic for data center lookup
* Added TriggerWebJobs to enable logic to force web job execution

# June 8, 2017

* Made changes to search query strings in preparation for Azure Search
* Cleaned up how titles are displayed in campaigns
* Cleaned up Contact Detail options to use drop down to selecct status

# June 7, 2017

* Added support for opt out on contacts.
* Fixed bug with how email merges get performed and cached

# June 3, 2017

* Remove campaign functionaliy was marking lead as rejected, when should have been deleted
* Update lead stats job to flag bounced contacts
* Add Bounced status for Contact status
* Add Account class initial check-in
* Add AccountId and Account APIs on Contact objet
* Update import logic to flag imports as 'imported' and ignore exceptions
* Reformat email activity item SQL
* Add AccountId to lead
* Add account not found exxcption to lightning exceptions
* Add /Account controller and AccountModel
* Removed existing account functionality to move to admin controller
* Add Index and Detail for Account controller
* Updated Remove Lead logic to delete not mark as rejected

# June 1, 2017

* Updated logic in web forms javascript to detect if Recaptcha script is already loaded.
* Added a 404 check in localhost mode for debugging
* Fixed a bug in web form slug check that was looking for null and not empty string
* Added async event handler on request demo button to dailystory.com to verify functionality