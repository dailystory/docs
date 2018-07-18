{
	title: 'July 2018 Product Update',
	description: 'Product Updates for July 2018'
}
# DailyStory Product Updates for July 2018
## July 16, 2018
* Refactor: process link tracking queues
* Enhancement: support for Google GeoCoding APIs
* Refactor: force tenant data center in email
* Refactor: log account not found exceptions
* Refactor: look up address to get geocode
* Refactor: side by wide display
* Refactor: add in support to search selectors for contact search
* Bug: gallery emails had a bad link
* Refactor: add close option to test popup


## July 15, 2018
* Bug: WordPress forms can cause a DSId not to get written.
* Enhancement: Better logging for exception handling in CMS
* Enhancement: Import search selectors from CSV

## July 13, 2018
* Refactor: Improvements to SalesforceSync job
* Refactor: Contact cache
* Refactor: email address formatting to handle aliases
* Bug: only add contacts to a segment if the contact is active on import
* Enhancement: whitelabel domain work
* Bug: Exception with short url names that start with f can confict with forms in cms
 
## July 11, 2018
* Enhancement: better field validation for contacts
* Enhancement: improvements to contact import auto-add to segment
* Refactor: folded ProcessContactQueue code into ContactQueueItem
* Enhancement: whitelabel domain 

## July 10, 2018
* Enhancement: Added skip rules for Workflow
* Enhancement: Added search selectors
* Bug: fixed bug in popup that caused caching conflict
* Enhancement: Added search selectors to admin
* Enhancement: Added better error message in popup javascript
* Enhancement: added support for rules in workflow
* Enhancement: updated workflow UX to use MD checkbox
* Bug: fake lead caused email links to break
* Enhancement: added IsIndexed check to GraphField
* Enhancement: better exception handling for Domain

## July 6, 2018
* Refactor: EmailSend and EmailStatus queues
* Bug: email activity item regression that wasn't updating delivery stats for emails
* Enhancement: LinkTrackingLead for unique url generation for SMS
* Refactor: updated text messaging and tests
* Refactor: enhancements to Twilio integration

## July 5, 2018
* Refactor: Convert campaign management to use SearchFilters
* Enhancement: add field graph support to contact
* Refactor: Handlebars and better exception management
* Refactor: add count to SearchFilter
* Refactor: CSS updates to admin
* Refactor: better exception management for failing to save/send emails
* Refactor: reporting improvement to campaign assets
* Refactor: additional support for whitelabel domains
* Refactor: validation on email save improvements
* Refactor: Improve email validation
* Bug: dates not showing in campaign email hoverover

## July 4, 2018
* Bug: DailyDigest default should be false
* Refactor: Uri extensions for StartupAuth to support white label domains
* Bug: Social media Image may not always be set
* Bug: Handle trial vs login
* Refactor: Improvements to contact search
* Refactor: Remove dependency on ds_tenant_datacenter

## July 1, 2018
* Bug: campaign id wouldn't get saved for popup on initial creation
* Enhancement: add waiting UX to choose tenant
* Enhancement: better tenant management for field graph and license
* Bug: email address validation could get trimmed
* Refactor: convert Mailgun to use queues to send email faster
* Refactor: updates to campaigns for tests
* Refactor: content pages caching
* Refactor: cryptography remove some public methods
* Bug: contact import sholdn't fail on nulls
* Bug: contact import convert items to bools
* Refactor: Email Send Queue and task management in Email
* Enhancement: add email status queue
* Enhancement: add email send queue
* Refactor: track campaign id in Graph Field
* Refactor: Email Activity Item singleton
* Bug: ReportBase was using times in days remaining calculation
* Bug: Search filter added point
* Refactor: convert Domain to use tenantUID for caching
* Refactor: updates to popup for tests
* Refactor: convert Email Workflow Rule to use Send Queue for emails.