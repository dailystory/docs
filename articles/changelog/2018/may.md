{
	title: 'May 2018 Product Update',
	description: 'Product Updates for May 2018'
}
# DailyStory Product Updates for May 2018
## May 24, 2018
* Feature: add author name, image, etc. to social card
* Refactor: optimize social css
* Refactor: convert social to model
* Refactor: style social cards

## May 23, 2018
* Feature: add ability to set a campaign to auto-qualify leads
* Feature: add date formatter for Tomorrow
* Feature: add open graph class for open graph lookups; used by social media
* Bug: add check for invalid key in rule engine
* Feature: social media posting, oauth libraries and more for LinkedIn and Twitter
* Bug: removed @sm from email validation even if it conflicts with css scrapes
* Bug: wait until rule was setting class member variable and causing rule to fail in edge cases
* Refactor: updated to integrations library; add support for LinkedIn and Twitter
* Feature: added SyncSocialMedia job
* Refactor: new bundles
* Refactor: update CSS libraries
* Feature: added social media account management in admin UX
* Bug: better mobile support in admin UX
* Refactor: WebForm UX new campaign selector and async requests
* Bug: problem when removing leads or contacts removed the wrong element
* Feature: added support to enable end user to select LinkedIn organizations for social media

## May 10, 2018
* Feature: Social Media posting
* Bug: Email reporting export delivery report
* Bug: potential bug in DS script / regression with iOS

## May 8, 2018
* Refactor: clean up and comment code
* Feature: stubbed in Social Media
* Bug: fixed bug with domain lookup
* Bug: Add check in DS script to skip older browsers
* Bug: Add logging for Microsoft authentication

## May 6, 2018
* Style updates
* Refactor: Admin user management
* Refactor: Improvements to daily digest
* Bug: fixes to link summary reports

## May 3, 2018
* Bug: Total active check in Campaign Stats

## May 2, 2018
* Enhancement: UX/CSS improvements and standardize on colors
* Enhancement: Added new notification when an existing user is added to a tenant
* Refactor: updated Joined Tenant logic
* Refactor: remove/add user to tenant
* Refactor: reworked oauth - another wonky behavior of openid
* Enhancement: added LinkedIn and Microsoft signin for invite UX

## May 1, 2018
* Enhancement: verify magic forms
* CSS and style improvements
* Feature: Twitter integration
* Updated API for SMS
* Refactor: Removed campaign types
* Bug: hopefully finally fixed MS auto-login bug
* Bug: clear timeout when magic form succeeds
* Enhancement: add text message to workflow
* Enhancement: Daily DIgest
* Enhancement: better orphaned link handling
* Enhancement: added urlhash to content pages for faster lookups
* Enhancement: remove DS logo from tenant notification emails that don't have a logo set
* Refactor: continued refactor of CampaignStats
* Bug: check for empty phone number before sending text messages
* Enhancement: Sms workflow rule