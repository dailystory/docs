{
	title: 'April 2020 Product Update',
	description: 'Product Updates for April 2020'
}
# DailyStory Product Updates for April 2020
## April 30, 2020
* refactor properties class to common classes
* modify ranged search filter to be inclusive on dates
* refactor search filter and update for inclusive dates
* remove old license contraints
* updates to weave installer
* add routes for dropdownlist populating efficiency
* bug in autopilot campaign links
* refactor split2 to remove javascript
* update to use new dropdown list apis
* project clean up
* updates to weave installer
* refactor weave properties
* fix bug with form2
* add additional contact fields to search
* add mobile phone to search and other updates

## April 29, 2020
* remove the displayimport url param when seen
* bug in import wireup for new start page
* updates to advanced search v2
* set count of matching records
* encode uri components
* remove search start
* support select2 tags
* added support for additional search filters

## April 28, 2020
* update to latest version of flowy and merge in changes
* age range updates to handle 21
* search v2 updates
* bug in advanced search for doubles
* always reset the pick list table
* updates for advanced search v2
* update common api calls to use promises
* remove and re-order datatable css library load order
* decode search components for search v2
* handle uri encoding in search v2

## April 27, 2020
* add support for canRender as some blocks should only be allowed once
* Return lead graph fields when we have a campaign id
* add funnel controller
* Add Campaign property to workflows
* Show campaign name when viewing all automations
* remove unused api and allow null campaign id for webforms all
* iteration on contact search v2

## April 26, 2020
* parse guids and convert to dsid format
* updates to weave installer for new fields
* updates to designer css

## April 25, 2020
* bug with loading in file manager modal
* css updates

## April 24, 2020
* update graph field picklist to store name value json array
* updates and refactor for contact import in prep for supporting mobile number as alternative key
* updates to common functions for handling phone number validation
* standarize phone number format
* updates to allow mobile phone or email as a contact key
* validation for phone numbers
* Email no longer required to save a contact
* contact map file validation for email or mobile phone
* contact import ux validates on email or mobile phone
* update picklists for custom fields

## April 23, 2020
* updates to web form to manage picklist
* add pick list ux to graph
* bug on integrations trim id
* standardize picklist table name
* standardize picklist css
* magic form path bug for home pages

## April 22, 2020
* bug in regex to match css for single or double quote
* update web form url paths
* simplify html designer for content pages
* add support for Weave integration
* trial check should bypass ip check if not a free email host
* update installer to setup weave custom fields
* Bug handling index of to in ranged search with names like totalorders

## April 21, 2020
* updates to web form controller for hosted forms v2
* Recaptcha site key needs to get set
* Add support for web forms v2 in landing pages
* handle cases where recaptcha is not enabled
* set recaptcha in landing pages
* Bug with page designer that causes images to always expand to 100%
* upgrade to webforms v2
* web form message not getting set

## April 20, 2020
* bug in lead graph when zero records
* remove redundant api controllers
* bug with pager displaying twice in email list
* bug in tracking links with custom limit
* bug in sql for source list

## April 19, 2020
* update to campaign stats api
* Add support for v2 forms in web form designer
* bug in how mapped fields were getting set in web forms v2
* updates to handle webforms v2 in CMS
* supadd additiona web form typesport v1 and v2 form items in web forms v2 designers
* remove member limits and clean up text message credits
* add additiona web form types
* handle urls for v1 and v2 web forms
* removed license limits on number of users

## April 17, 2020
* performance work around campaign and lead stats
* convert to left outer join for stats views
* bug with comma in number
* work on campaign api
* updates to web form designer v2

## April 16, 2020
* Update whitelabel logic
* update campaign stats api endpoints to v1
* add campaign dashboard report
* update with additional RhinoFit fields
* set isfirsttime for first time the job is registered
* updates to RhinoFit integration with new fields and error handling

## April 15, 2020
* remove campaign license limits
* Add new license types: start up, standard and growth
* updates to RhinoFit integration
* updates to upgrade and license usage report
* bug in old campaign license check path
* bug in twilio status lookup for text messages
* updates to web forms designer v2

## April 14, 2020
* bug in text message designer editor
* Updates to licensing and how text messages credits are counted
* RhinoFit install/uninstaller
* updates to licensing UX
* add support for RhinoFit in UX

## April 13, 2020
* RhinoFit integration
* Handle null name fields in email

## April 10, 2020
* zapier endpoint needs to force authentication

## April 9, 2020
* Performance improvments to lead and contact activity
* update contact activity ux

## April 8, 2020
* camapign fields in sidebar
* ensure table is setup before trying to setup paging
* Clicking an email report, such as opens, shouldn't constrain by date
* refactor mailgun api to add support for AMP emails

## April 7, 2020
* updates to contacts data table
* handle case where row doesn't exist
* handle clear behavior in datatables 
* graph field api returns full contact property set
* support new graph api to populate contact field list
* updates to web form designer v2 blocks
* remove replaced api for graph
* updates to manage campaign and contact graph
* getgraphasync should always return by id

## April 6, 2020
* remove text message settings
* update trial creation logic to block certain countries
* bug in common tags lookup
* add tags to advanced search v1
* update trials to use tags
* bug with tag ux new tags not linked properly

## April 4, 2020
* refactor new lead notification method

## April 3, 2020
* web form v2 designer updates
* redirect hash support for email tracking
* bug with internal email check on trials
* log sms clicks to sms click queue
* bug generating internal lead id from base 64 encoded linkid
* update to text message reports for delivered and clicks
* bug when clicking on report for email in list
* iteration on webforms designer v2
* fix breadcrumb bug in push ux
* add version to track version for web forms v2
* set focus on advanced search
* Add menu options for branch

## April 2, 2020
* support select name value pairs in web form designer v2
* web form submit action option
* change location controller to cancel vs delete
* stub out appointment create/edit
* updates to modal timeslot editor
* fix bugs with how locations are retrieved
* separate email url hash path
* merge Base64 encode url email

## April 1, 2020
* Clean to trial creation process exception handling
* Typos and updates to NeverBounce
* bug in insert for timeslots
* When creating a new autopilot automation the disabled state needs to be shown
* iteration on web form designer v2
* add recaptcha design element for web form designer
* refactor how salesforce handles custom object lookups
* updates salesforce to pull custom object by last updated in batch
