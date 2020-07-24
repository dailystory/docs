# DailyStory Product Updates for July 2020
## July 24, 2020
* allow emails to support delivery time
* convert mailgun to httpclient
* add assign task action to automation
* throw exception in automation when block is invalid

## July 23, 2020
* support donotcontactuntil and lastcontacted for date triggers
* add tag and add segment in automation shouldn't be called if not provided
* add trigger for when points matches
* fix various minor bugs in autopilot designers
* move change status to api
* fix api paths for segments

## July 22, 2020
* setup birthday support for search
* parse regions for country
* search ux for birthday

## July 21, 2020
* better visual status for running/paused automations
* trigger when opted out
* order tags by name
* allow creation of tags in automation UX
* allow creation of segments in automation UX

## July 20, 2020
* bug witth block lookup using array index instead of id
* import handler for automation
* handle import for automations
* bug with non image files attempting to set a preview image
* more bugs with block index and ids
* allow import from a url for automations
* add helper method to download file

## July 19, 2020
* add whennone automation trigger
* add automation action for goto

## July 16, 2020
* add UX automation trigger for register device
* trigger when device is registered
* enable some triggers to allow for leads to be created if they don't exist
* add support for exporting automations

## July 15, 2020
* add delete button on autopilot block properties
* update naming conventions for conditions in autopilot
* add support for when tag added/removed triggers
* update text used in conditions for autopilot

## July 14, 2020
* update MBO sync to force sync clients with memberships
* handle case when mbo date to sync back is null

## July 13, 2020
* Remove create workflow options

## July 11, 2020
* updates and refactor for automation test coverage on actions
## July 10, 2020
* bug with email templates forcing unlock html
* bug in save path for retarget pixel
* bug with case insensitive comparison for text replies
* ux updates to better identify automation items
* if do not send until date is set, return a waiting status on the message
* update automation action for do not contact until

## July 9, 2020
* add ux for has tag to automation
* support ninja forms in magic forms
* bug in remove tag name
* bug with left outer join on emails

## July 8, 2020
* add condition to check if has tag
* bug with returning leads in automation

## July 7, 2020
* streamline segment creation flow from search
* handle Twilio exception in workflows
* reporting range issue in conversion funnel

## July 6, 2020
* Set date last sent for email from queue send
* Fields ending in _code won't have casing changed

## July 3, 2020
* fix compiler warnings
* updates for email sending and reporting performance
* better logging for scheduled messages
* stream line how email activity is updated
* longer timeout on segments
* performance improvements

## July 2, 2020
* search dates must contain zulu
* convert email reports to use view
* email templates should retrieve from view
* update sync twilio with dependent library

## July 1, 2020
* dsids search filter must use order by
* bug to handle date ranges in filters
* remove local tinymce references
* migrate to tinymce 5 and CDN
* hide table borders in mce editor
