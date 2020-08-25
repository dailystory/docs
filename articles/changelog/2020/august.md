# DailyStory Product Updates for July 2020
## August 25, 2020
* add support for import/export segments
* bug more unwinding of /v1 reports routes
* updates to support autopilot and segment templates

## August 24, 2020
* bad controller paths in the sms report
* updates to funnels
* Renamed OffsetTimezoneFromUTC to ConvertUTCToLocalTimezone
* Bug with email queue using wrong conversion for UTC to local time
* track funnel associated with the conversion

## August 21, 2020
* added ReportCsvHelper to easily convert DataTable to CSV
* Add export SMS replies and paging in UX
* refactor to improve contact reindexing performance
* Remove punctuation from sms keyword for processing
* Manage tags shouldn't require administrator privlidges
* reports shouldn't be versioned
* bug api path updates from refactor
* updates for funnels to include additional detail

## August 20, 2020
* bug set mobile number when looking up lead
* progressive lookup by dsid, email and then mobile number
* remove updates to campaign_workflows
* add trigger to run when leads are removed from a segment

## August 19, 2020
* minor bugs and ux improvements to text message deliverability score
* bug join table to ensure logs exist
* add birthday to contact record ux
* bug don't display example.com emails in ux
* allow type jpeg for image picker
* add category just for a URL

## August 18, 2020
* better handle 30007 codes from Twilio
* expand length of text message body to accomodate long URLs
* add spam checker
* add support for deliverability scoring when creating a text message
* add lookup for phone number to Twilio sync
* don't process text messages with whenall

## August 15, 2020
* bug with how scheduler calculated stats

## August 14, 2020
* set favicon, description, author and  keywords in pages
* set generator an og:site_name in meta tags for pages
* bug city wasn't included in advanced search
* add support for select2 in automation ux dropdowns
* support select2 for tag related items in automation
* support select2 for segment related items in automation
* add select2 for campaigns in automation and fix bug with selected item
* use select2 for user dropdowns in automation

## August 13, 2020
* updates and improvements to multivariate emails
* updates for how neverbounce handled exceptions for parallel processing
* enhance neverbounce to run processes in parallel
* only emails of type email can be scheduled
* bug with start trigger checking logic
* add conditions for is in segment and is in campaign

## August 12, 2020
* Refactor email revisions into asset revisions

## August 11, 2020
* stub for AMP emails
* save versions of emails

## August 10, 2020
* add support for email variants
* initial check in for multivariate support in ux

## August 8, 2020
* Shouldn't be able to create duplicate email senders
* Refactor for testing of managed senders
* Trigger automation when a tag is added in bulk add
* Add quick actions to campaigns

## August 7, 2020
* autorouted lead needed additional detail for notifications
* Add advanced option for emails to disable/enable click and open tracking
* Add bulk upsert for tags
* add support for adding tags during bulk import
* Add support for bulk add tags to contacts

## August 6, 2020
* updates to http helper
* initial check in for two factor auth support
* bug shouldn't be able to go to a go to step in automation
* set isStartTrigger to indicate that a trigger can only be used to start an automation
* Ability to access an asset's sub-menu from within the campaign with ...
* allow dynamic segment search criteria to be updated using search ux
* bug with duplicate column
* everyone is no longer selected by default and time is set to +1 hour for scheduler
* warning wasn't shown when 0 leads in campaign
* set email last sent date time
* Add Yelp as a built in social url for personalization and in settings
* clean up and refactor contact activity
* Add new action: add note
* move POST activity for contact to contact API

## August 5, 2020
* wildcard url matching trigger
* bug email conditions weren't defaulting to 72 hours
* allow email has clicked condition to use specific url
* check for specific click in email condition
* when removed from campaign also remove from automation
* bug in scheduler pre-send logic
* update dailydigest to use httphelper and not send on errors

## August 4, 2020
* return urls in email for automation
* check if a given url in an email is clicked or check for any click
* display segment stats when viewing members
* update trigger to allow for specifying the email link that was clicked
* return the links for a given email

## August 3, 2020
* do not allow same message to be scheduled within 1 hour

## August 2, 2020
* Refactor IsOptOutUrl to IsIgnoredForClickTracking
