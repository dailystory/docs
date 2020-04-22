{
	title: 'April 2020 Product Update',
	description: 'Product Updates for April 2020'
}
# DailyStory Product Updates for April 2020
## April 22, 2020
* bug in regex to match css for single or double quote
* update web form url paths
* simplify html designer for content pages
* add support for Weave integration
* trial check should bypass ip check if not a free email host

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
