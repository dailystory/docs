{
	title: 'March 2018 Product Update',
	description: 'Product Updates for March 2018'
}
# DailyStory Product Updates for March 2018
## March 24, 2018
* Massive refactor and compressed javascript and css files
* Feature: Add support for LinkedIn signin
* Feature: Added handlebars templating for content and emails
* Bug: Domain check in content pages on creation
* Refactor: Emails, EmailTemplate
* Feature: Lead and contact graphs
* Bug: licensing could sometimes inaccurately report campaign usage
* Refactor: Upgraded core packages
* Feature: Updated parser ignore list
* Feature: Updated domain list
* Feature: Added text messaging support with Twilio
* Feature: Updated domains to use dlysr.io
* Feature: Sms Workflow rule
* Feature: WaitUntil workflow rule
* Refactor: Updated integration packages
* Feature: Added verify credentials for Mailgun
* Feature: Added Twitter integration
* Refactor: Updated Workflows Job packages
* Test: Updated and added multiple unit tests
* Refactor: Updated Web packages
* Bug: fixed multiple CSS issues; standardized UX for date picker
* Feature: Added Twilio integration option in admin panel
* Refactor: Email API to follow standard of other APIs
* Feature: Added API for SMS
* Refactor: Email Controller
* Refactor: Clean up and standarization in web project for async task; removed unneeded files
* Refactor: JavaScript libraries for link tracking, email, text messaging and content pages
* Refactor: Better campaign selection and default behavior if only 1 campaign
* Feature: Added validation check for phone numbers
* Feature: Added WaitUntil Workflow step
* Bug: User preferences added validation on phone number

## March 19, 2018
* Bug: leads added before workflow would cause workflow to skip
* Bug: return success/fail from dequeue lead
* Feature: added support for date workflow item

## March 17, 2018
* Bug: postMessage origin check added
* Bug: ds change to use structured clone and pass origin
* Bug: Google Analytics tag on free trial page
* Add CORS header for progressive profile
* Bug: Origination in lead detail for link is incorrect format

## March 15, 2018
* Bug: New tenants should have a default timezone
* Bug: Licensing for sub-accounts
* Feature: Sort accounts by name alpha
* Bug: Mailgun credentials should support verification
* Feature: Verify tracking code
* Improvement: break early for license exceptions for email volume
* Added a check to see if tracking is active

## March 14, 2018
* Bug: opt out form; Submit is throwing an exception going to the wrong page.
* Improvement: Plain text option in emails shouldn't be "some content here"
* Bug: Emails using a template shouldn't have html body editing
* Feature: Campaign creation needs license check

## March 12, 2018
* Library updates
* Fix bug with adding all contacts to list
* Added lookup to parse base domain
* Updated email parser loops to use HashSets instead of arrays
* Additional validation checks for emails
* Better error handling for failed writes to web tracking queue

## March 8, 2018
* Fix some build warnings
* Add better dsid checking/validation

## March 4, 2018
* Refactor Parser
* Improvements to format percentages as part of reports
* More improvements to validation checks on emails
* Changed IsDuplicate check on leads to return the duplicate Id
* Added Nurturing as a LeadStatus type
* Added LoadStringArrayFromFile to Common class

## March 2, 2018
* Refactor email parser

## March 1, 2018
* Better Html stripping in Common formatter
* Refine keywords for identifying service providers
* Work on email parser
* Add email validation check in case we get a CSS rule