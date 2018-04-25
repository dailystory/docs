{
	title: 'April 2018 Product Update',
	description: 'Product Updates for April 2018'
}
# DailyStory Product Updates for April 2018
## April 24, 2018
* Refactor: Data Tables
* Refactor: Updated CSS for material forms
* Refactor: Remove description requirement for lists and campaigns
* Refactor: Better mobile support for Chooser
* Refactor: Campaign Create/Edit
* Bug: Campaign license check

## April 23, 2018
* Enhancement: Better handling for Lead Stats HasVisited
* Tests: added additional tests for HasVisited
* Package updates for jobs
* Enhancement: add support for LinkedIn sign up
* Enhancement: continue link tracking refactor
* Feature: added IconUrl to Tenant
* Feature: added check to User for multiple accounts
* Enhancement: improve mobile support in login
* Enhancement: added better account chooser for multi-account users
* Enhancement: add support for primary account

## April 22, 2018
* Bug: fix issues with campaign workflow returning false positives
* Bug: better handling for email validation with spammer emails
* Refactor: Remove some old code and build warnings
* Enhancement: prevent name collisions in magic forms
* Enhancement: improve landing page
* Enhancement: Added new reports KPISummary and Page Views
* Bug: fix miscelaneous responsive design issues


## April 20, 2018
* Update integrations version
* Bug: Better exception handling in SyncSalesforce
* Bug: Handle bad email addresses in workflow
	
## April 19, 2018
* Refactor: JSHint updates for magic forms
* Test: Test files for Magic Forms
* Refactor: Magic Forms support Query Strings
* Feature: Personalization in PreHeader
* Refactor: Forward Params
* Bug: bug in parse pathing for magic forms
* Feature: Campaign filter for email
* Refactor: JSHint update for link tracking
* Refactor: Refactor warning messages

## April 18, 2018
* Bug: bug with ace editor not properly encoding html
* Bug: leads that cilcked a tracking link we not getting assigned to the origin campaign.
* Enhancement: script bundles for leads
* Bug: lead detail links for paid search

## April 17, 2018
* Enhancement: updated Mailgun to include better support for bounce detail
* Bug: Allow preview option for email web view
* Enhancement: tracking links include retargeting if it exists

## April 16, 2018
* Refactor: Link Tracking
* Bug: Link Tracking double-asking for campaign
* Bug: Missing style on workflow
* Bug: error in about json
* Bug: edge case error handling empty nodes in email parser
* Enhancement: add support for reason for email bounce

## April 14, 2018
* Refactor: Link Tracking simplification
* Bug: fixed auth issue on forced logout could redirect to wrong url
* Refactor: Link tracking use async and add model

## April 13, 2018
* Enhancement: updated CSS styles
* Enhancement: date picker for link tracking only allows picking future dates
* Bug: url validation is case insensitive
* Enhancement: tightened up UX in admin settings for logo help text
* Enhancement: updated Contact Table for iPad
* Enhancement: updated save UX for iPad
* Enhancement: updated email UX for iPad
* Enhancement; updated Link Tracking JavaScript
* Enhancement: updated sidebar Admin CSS

## April 12, 2018
* Unit test updates
* Bug: fix paging when date selected for periscope
* Bug: Page templates

## April 11, 2018
* Feature: better about page with tenant uid when custom domain for validation
* Bug: update domain validation to check http or https
* Bug: form UX margin
* Enhancement: add mini error css
* Enhancement: add subdomain to admin
* Enhancement: add check if slug is unique
* Enhancement: don't require UIG in known domains
* Enhancement: updated alias ignore list
* Enhancement: added behavior to Domain object

## April 10, 2018
* Feature: working on LinkedIn single sign on
* Refactor: removed Workflow.css and integrated with forms
* Bug: Fixed multiple issues with workflow javascript dealing with date/time rule
* Bug: Fixed bugs with reporting on home page
* Bug: Fixed status check in score leads
* Feature: set titles in template pages from page title

## April 6, 2018
* Feature: add support to handle ROT13 encoded URLs
* Enhancement: add support to safely get extended properties from a contact
* Bug: changed sort order of graph field list
* Bug: clear cache on update lead
* Enhancement: style changes on form inputs
* Enhancement: removed box shadows from panels
* Enhancement: tightened up panel UX
* Enhancement: changed Lead API to use Update method and Save
* Refactor: updated Lead Create Edit screens to handle extended profile fields
* Enhancement: added link to campaigns in create edit for navigation
* Bug: fixed UX bug on lead detail mark as qualified button
* Bug: fixed bug in lead stats API

## April 5, 2018
* Feature: Add support for web view of email
* Enhancement: Add support for checking if test DSID is being used
* Enhancement: Moved EmailId to base class for merge tags webview
* Feature: Added merge tag for webview of emails
* Feature: Added preheader for emails
* Enhancement: set test DSID as public in Lead
* Bug: fixed some style issues with on/off button
* Feature: add support for preheader and webview to email view page

## April 1, 2018
* Feature: Profile graph data import initial check in
* Bug: Fixed bug in email templating
* Feature: Added graph and graph data types
* Bug: Fixed bug in case sensive matching for Hostinfo
* Feature: Added method to update lead
* Feature: Added merge lead extended properties and contact extended properties when working with a lead
* Enhancement: sorting fields used on import
* Bug: logo generation for notifications when no tenant is present/known
* Enhancement: email parser to support multiple separators
* Enhancement: added new email types
* Enhancement: added profile rule to read values from lead extended properties (graph)
* Enhancement: updated rule selector to pull list of graph fields for campaign when displaying the rule selector
* Enhancement: rule engine now supports rules for profile graph
* Enhancement: added functionality to verify credit card
* Enhancement: added exception type for handling issues with credit card charges
* Refactor: removed some dead code with trials
* Enhancement: added a trigger to trigger profile graph import
* Feature: initial check in bulk import profile data job
* Bug: fixed automations to check lead last modified date for when to run
* Unit test updates
* Refactor: additional bundles
* Enhancement: card verification in admin UX
* Feature: Added Field to Campagign API
* Enhancement: converted score and automation views to async
* Enhancement: profile graph UX for Contacts and Leads
* Enhancement: Removed/replaces User.Tenant with User.GetTenant to better handle multi account
* Enhancement: updated rule model to support async loading
* Enhancement: updated rules.js to handle operator type any
* Enhancement: added UX for picking graph file and managing graph fields