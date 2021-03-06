{
	title: 'March 2020 Product Update',
	description: 'Product Updates for March 2020'
}
# DailyStory Product Updates for March 2020
## March 31, 2020
* initial support for rte in web form designer
* conditions and triggers for text message clicks
* refactor textmessagelink
* update textmessage click queue item for automations
* standardize automation item keys
* update text message valid send time to start at 500a
* updates to web form designer v2
* rename time slot modal and upates
* typo in select name
* initialize the timeslot modal
* API to update a timeslot

## March 30, 2020
* update not found message for dslnk.co
* update sms designer ux to support url shortener
* clean up formatting html for push designer
* additional twilio enum types
* add support for base 62 encoding with capitalization support
* refactor text messaging to support redirect tracking links
* click tracking is on by default for new text messages
* set help and handle label when populated in input box for webforms designer

## March 29, 2020
* support export method for graph fields
* refactor timeslot modal
* update to campaign and contact graphs for export

## March 28, 2020
* bug when popup path included full url
* refactor how labels are handled in webform designer v2a
* remove render v1 from label
* bug segment shouldn't exclude example.com emails for stats
* handle additional Twilio codes
* update selection and drag styles in web forms designer
* make sure Campaign is set if utm campaign is set

## March 27, 2020
* handle deselecting when clicking outside of web form designer
* updates to web form designer
* webform designer components
* create/update time slot on location modal
* standardize checks for @test and @example emails
* set isemailenabled when updating a contact
* set isemailenabled false when set to example
* timeslot requrest start and end date
* instrutions property on location
* handle import from webforms v1

## March 26, 2020
* fix link paths to delivered emails
* webform designer v2 updates
* appointment time slots must support start and end dates
* schedule an appointment
* appointment exceptions
* Location is open and get location timeslots
* mindbody handle client services that get used up

## March 25, 2020
* Emails sent through workflow needs to honor email isTransactional state
* update for returning all locations
* delete a time slot
* refactor web form ux

## March 24, 2020
* handle exceptions in Twilio post instead of returning message
* update time picker style
* updates to locations
* support for custom object field lookups in SFDC
* add support for add/remove tags in autopilot
* refactor timeslots for locations
* handle timeslots in ux
* bug Import link on side bar menu of contacts does not work

## March 23, 2020
* add support for appointment location
* location sort and skip lists

## March 22, 2020
* handle additional whitelabel domains
* initial checkin for appointments
* add JSON properties to address

## March 21, 2020
* optimize how geo location lookups are performed

## March 20, 2020
* updates for salesforce integration sync
* updates to ip address lookup
* updates to social media publishing ux
* refactor to clean up social media accounts
* hardcode whitelable for itm
* prevent over querying of open street maps

## March 19, 2020
* move social media sync logic into core
* refactor social media ux and move to datatable
* add ip address helper

## March 18, 2020
* tracking links and users weren't getting properly set for class of service
* move url helper and other improvements
* add support to storage for utmcampaign
* refactor how emails build links for utm codes and tracking tags
* set utm in campaign ux

## March 17, 2020
* status of automation to show is running or not
* add url helper for working with utm codes
* Add utmsource to campaign

## March 16, 2020
* bug when export search s is not set in querystring default to all
* more datatable updates
* fix breadcrumb separator
* add filter for segments
* updates for search for improvements to contacts and segment search

## March 15, 2020
* add validations
* check if text message keyword already exists
* organize for unit tests

## March 14, 2020
* use tag id when displaying tags in search
* add tag to contact document
* update last indexed when tag is added/removed from contact

## March 13, 2020
* add support for text message keywords
* bug in save and close with screenshot logic
* text message keyword activity ux
* set origin data on leads created through text message keywords
* process keywords before start words
* create lead should capture origin name, and lead source id
* various bugs in tags
* updates in UX for supporting contact tags
* clear tag cache on update

## March 12, 2020
* handle tracking link license exception
* convert to explicit send test method for emails
* remove greatest deferred date
* don't modify raw html if designer isn't used
* add better support for transactional flagged emails
* bug in url path
* campaign selector should call callback when set campaign id via url
* lead status action should allow 0
* add ux for setting email as transactional
* set conditions when occurs vs waiting until process date
* set condition for email open and click
* set transactional status for email preview
* add ux for text message keywords

## March 10, 2020
* save lead on keyword creation
* add bbcs integration UX
* installer for bbcs
* add support for bbcs eligibility
* add istransactional email flag
* set webform to 0 on clone
* integration fields for bbcs

## March 9, 2020
* fix sort bug on conversions
* show magic form conversions

## March 8, 2020
* sms keyword support
* check if dsid is in campaign

## March 5, 2020
* group buttons into div
* refactor isavailable to isslugunique
* page api and refactor how slugs are handled
* clean up slgu api names
* add update slug to content pages
* design buttons modeled after email design buttons for pages
* remove claims check for getting segments
* remove segment caching
* published links can't change url slugs
* enforce slug length and allowed characters
* merge needs to update date_last_indexed for inserts

## March 4, 2020
* issue with loading sequence when campaign not set
* Lead names in campaigns not populating
* reduce request size of member of for segments
* api and end points for new shortened links
* add license checks and updates for link shortner
* move web page parser/preview to class
* revert asset path changes

## March 3, 2020
* bug in block builder
* more advanced search updates

## March 2, 2020
* return a data table model for contacts
* custom pager
* handle case when paging is serverside to not redraw
* handle when search text is passed in via query stringI
* bug with Mc and Mac handling
* add GetTotalRecords
* set tenantid
* bug handling automation delete redirect
* clean up search and decode uri
* fix links and button names to standard format
* refactor how we deal with & in advanced search
* revert email list goes to edit
