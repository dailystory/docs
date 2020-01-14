{
	title: 'January 2020 Product Update',
	description: 'Product Updates for January 2020'
}
# DailyStory Product Updates for January 2020
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
