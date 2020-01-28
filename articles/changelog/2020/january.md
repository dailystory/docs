{
	title: 'January 2020 Product Update',
	description: 'Product Updates for January 2020'
}
# DailyStory Product Updates for January 2020
## January 27, 2020
* Refactor: wait block to use single date/time
* Refactor: re-organize workflow controller
* Refactor: use enum types for blocks in workflow
* Refactor: updates for saving workflow
* Refator: block base sets step action type from block name
* Refactor: fold enum into single StepAction type
* Refactor: don't bring back design for list of workflows
* Refactor: workflow v2 api for get/post workflows
* Refactor: return light model for javascript calback
* Refactor: continue to align names with enums
* Refactor: load/save workflows in designer
* Refactor: bring in flowy source
* Bug: set proper name for enum matching and handle arrays in props
* Refactor: enum name matching
* Refactor: remove dead code
* Refactor: add drag handle to blocks
* Refactor: add delete steps method
* Refactor: undo block drag updates
* Refactor: only allow drag after selected
* Refactor: pass step directly to action and let action determine values
* Refactor: return null instead of exception for not found step
* Bug: handle when no waittime is set on opened email
* Refactor: convert action to return step action

## January 26, 2020
* Refactor: match block type to AutomationStepType
* Refactor: rename AutomationStepType to StepType
* Refactor: clean up workflow vnext ux
* Refactor: set step type and step id when exporting blocks

## January 24, 2020
* Refactor: update naming conventions for workflow blocks to match types
* Refactor: another massive code refactor to workflow; UX v1 nearly complete

## January 23, 2020
* Refactor: enforce rules around child/parent relationships in workflox UX
* Refactor: more updates to workfow vnext ux
* Refactor: ux updates for workflow vnext designer
* Refactor: split blocks into individual files; optimize loads

## January 22, 2020
* Refactor: normalize naming convention for Workflow actions
* Refactor: update page view trigger to include 1 day
* Refactor: re-org and unit test all of workflow class
* Refactor: simplify logic for base send date time condition
* Refactor: set specific enum values
* Refactor: add support for additional trigger types
* Bug: catch runtime exception for bad personalization tags
* Bug: Update email preview text following Facebook's example
* Refactor: continued updates to workflow ux designer branch

## January 21, 2020
* Refactor: continue to refactor workflow v2
* Refactor: update Rejected enum id for easier exclude
* Refactor: remove old workflow controller
* Refactor: rename classses and add support for Action in automation

## January 20, 2020
* Refactor: mark as delivered by default
* Bug: security operation issue with html2canvas on Safari
* Refactor: click open queue to use bulk sql
* Refactor: workflow redesign with multiple steps and workflows
* Refactor: cleanup workflow for v2

## January 15, 2020
* Refactor: updates to new workflow designer
* Refactor: update clickopen queue job to run every 10 min
* Refactor: move process queue for better unit testing
* Refactor: tracking link api routes
* Refactor: named links, status, etc. for rules enginea
* Refactor: handled specified dates and ints; add tracking links rules check
* Refactor: modify automation to use contact last modified
* Refactor: add support for equal on dates and link clicked
* Bug: cors not set for image proxy'
* Refactor: more rules.js clean up
* Refactor: start removing jquery dependency
* Refactor: ensure email can get reset in MINDBODY
* Refactor: degree37 do not contact until logic

## January 14, 2020
* Refactor: update rules javascript libs
* Refactor: normalize automation and workflow actions
* Refactor: add lookup for lead by dsid
* Refactor: class rename for scoring and automation on leads
* Bug: check duplicate id check on lead wasn't setting status
* Refactor: throw exception if campaignid <= 0
* Refactor: campaign action selector for rules
* Refactor: support rule actions with populated drop downs
* Refactor: better handle open, clicks, views from rules engine
* Refactor: incremental updates to workflow designer
* Refactor: begin to add snap to logic

## January 13, 2020
* Refactor: automations job
* Refactor: namespace update to .Automation
* Refactor: clean up and refactor
* Refactor: campaign rules and automations
* Refactor: Change advanced search to more options
* Refactor: start implmentation of new workflow designer
* Refactor: handle case where message is not found/ready yet

## January 10, 2020
* Refactor: contacts api, permission and exports
* Refactor: update maintenance job
* Refactor: update maintenance job
* Refactor: re-org code and add support for permanent delete
* Refactor: mark expired tenants as deleted
* Refactor: handle case where tenant no longer exists

## January 9, 2020
* Refactor: message validation for frequency and transactional messaging
* Bug: handle workflow step case where segment no longer exists
* Refactor: add push audience dashboard
* Refactor: update email dashboard with demographics
* Refactor: convert file manager to use view
* Refactor: updates to file manager

## January 8, 2020
* Refactor: push notification api name
* Refactor: push notifications ux
* Refactor: workflow interactions
* Refactor: clean up workflow steps
* Refactor: remove Code from ApiStatusResponse
* Refactor: handle scheduled messages that cannot be sent
* Refactor: utility method to help find greatest date
* Refactor: api tokens larger
* Refactor: move api token management into api
* Refactor: remove picasa lookup for avatars

## January 7, 2020
* Bug: included localhost in path
* Refactor: restructure push notification api
* Refactor: sort push notifications alpha
* Refactor: improve naming and logic for retrieving a workflow step
* Refactor: workflow api
* Refactor: clean up push api
* Refactor: sms api send single

## January 6, 2020
* Refactor: order text messages in api by name
* Refactor: only sent workflows when campaign is valid
* Refactor: validate emails sent through queue
* Refactor: normalize apis
* Refactor: remove mailchimp workflow
* Refactor: add import to main nav
* Refactor: order emails by name

## January 3, 2020
* Refactor: clean up workflow
* Refactor: job logic into workflow
* Bug: section was commented out
* Bug: password check shouldn't show ux
