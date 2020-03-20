{
	title: 'March 2020 Product Update',
	description: 'Product Updates for March 2020'
}
# DailyStory Product Updates for March 2020
## March 20, 2020
* updates for salesforce integration sync
* updates to ip address lookup
* updates to social media publishing ux

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
