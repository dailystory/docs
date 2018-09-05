{
	title: 'August 2018 Product Update',
	description: 'Product Updates for August 2018'
}
# DailyStory Product Updates for August 2018
## August 30, 2018
* Feature: grapejs initial check-in
* Bug: in phone number edit contact floater
* Refactor: Design editors for email and content
* Feature: roles updates
* Bug: white label error handler
* Refactor: updates to designer

## August 29, 2018
* Refactor: update binary dependencies 
* Refactor: gloabl replace of error message
* Refactor: Email and Content editor to design view
* Refactor: SetAccount owner name change to add async
* Refactor: UserPreferenceModel and AdminSettingsModel
* Bug: handle error in text message save

## August 25, 2018
* Bug: save on change broke save button
* Bug: API Contact Controller calling Save incorrectly.
* Refactor: api exceptions should always return json

## August 24, 2018
* Refactor: add modified since to rule selector for perf improvement
* Refactor: Move HasVisited logic to custom rule for perf improvement
* Bug: tenantuid not included in SQL for social
* Bug: email rules when send immediately, but a date is specified.
* Refactor: add color pickers to tinymce
* Refactor: Content consistency edits
* Bug: lead campaign id could be set incorrectly
* Refactor: Move roles to javascript file

## August 23, 2018
* Bug: reenable sub accounts in admin
* Refactor: Clean up message text
* Bug: lists enumeration was using emails
* Refactor: fold campaign javascript into separate file
* Refactor: white label help links in UX
* Enhancement: continue UX work on roles
* Refactor: rename ContactList workflow to Segment workflow
* Bug: empty workflows shouldn't throw
* Enhancement: get users not in role
* Bug: owner id not being set correctly for campaigns
* Enhancement: stub support for optout sms and push
* Feature: initial check in of MindBody api support
* Bug: social media could repost if channel id not set
* Bug: contact document segment builder added filter twice
* Bug: handle google api exceeded api query limit

## August 22, 2018
* Feature: Clone campaigns, popups, emails and workflow
* Bug: Queued email sends didn't update contacted date
* Enhancement: Add support for setting parent id when creating a tenant
* Refactor: pass tenant when creating a campaign
* Bug: show error message if creating an account fails
* Bug: popups and magic forms shouldn't run if the campaign is not active

## August 20, 2018
* Bug: bug in lead export from campaign
* Bug: file collisions on upload
* Feature: begin manage roles UX
* Feature: add reporting for content pages
* Enhancement: set campaign id on copy for poups
* Refactor: fold role permissions into ds_roles

## August 19, 2018
* Feature: support for roles and claims
* Refactor: return absolute uri from image store

## August 17, 2018
* Bug: bug in copy webform not reseting id
* Bug: bug in image management not properly quoting css url
* Feature: add link summary report
* Feature: update click path tracking

## August 13, 2018
* Bug: convert timeline icons to use font awesome
* Feature: add RegisterDevice API to Contact
* Feature: begin work to support Grape JS editor
* Refactor: rename from exit intent to popup
* Feature: add support for Twilio push notifications
* Refactor: better error handling for templating