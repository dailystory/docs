# DailyStory Product Updates for October 2020
## October 26, 2020
* Add batch update to graph fields
* popover stats in scheduler

## October 25, 2020
* Favorites aren't updated for rows in DataTable
* Move graph field to api driven

## October 24, 2020
* Add support for personalization picker
* Automations in campaigns should clone
* Convert edit email html to use api for amp emails

## October 23, 2020
* Update search filter to support is numeric
* Bug handle check for null tag
* Remove old paged leads from campaign view

## October 22, 2020
* Update CheckHasWorkflowAsync to use autopilot
* Bug with handling "any" condition on opt out trigger
* Refactor naming and add condition for has submitted popup
* Add support for has submitted Magic Form condition
* Add condition for has visited page
* Add support for WhenApiIsCalledAsync trigger
* Bug with handling empty strings in import

## October 21, 2020
* Improvements to text message spam checker
* Create trial for onetool users
* Bug in automation when date do not conact is set for sms
* remove old workflow route
* Bug with bounds checking on scheduled dates
* Bug with null check on rss summary
* Add percentages to export reports
* Add text message export button similar to email
* Iteration on Tag users in bulk
* support for bulk add/remove in api
* Support for bulk add/remove in tag component
* Add support for additional social icons

## October 19, 2020
* padding and spacing issues with emails that are image only
* remove full width on images and add block
* Support filtering of leads in campaign view
* Bug with no breaking space
* Better format description on RSS feed

## October 17, 2020
* Link SMS reports to leads not contacts
* Handle ellipses and space breaks
* Enable limiting text returned from RSS results
* Add DailyStory specific Css classes to email css
* set css classes for mobile behavior on images in designer
* add support for pre-defined templates for rss

## October 16, 2020
* Extract contact GetGraph to tenant
* Add render async to content page for handle bar personalization
* Deprioritize updating dynamic segments when multiple items in task queue
* Update graph fields during sync for Weave
* Landing Page Footer in Designer does not have built in personalization
* Expand udf strings from 10 to 15

## October 15, 2020
* bug with handling picklist with empty string

## October 14, 2020
* Update to use SearchUtil Parse Search text
* additional email designer layouts
* Move Segment stats to top of page & add "math" line item(s) for who's eligible
* Add support for email enabled in segments
* add export and create segment to top of page
* trim search results what parsing
* Add "Send Email" to advanced options menu form within the assets list of a campaign

## October 13, 2020
* Remove Terms from views
* Handle case where firstname was single character
* Convert text message trigger to use message id vs reply text
* Sort file manage picker by date created vs. alpha
* Pattern web form designer after automation and bug fixes
* Improve math calculations on stats for segments
* Ability to edit Email Templates in the Designer

## October 8, 2020
* Standarize the mobile number before performing validation check
* Remove lead terms

## October 7, 2020
* add support for better placeholders in designer
* Add required indicator on forms
* Word/Letter case revisions accepted in contact records for imports

## October 6, 2020
* Support changing the size of the social icons
* updates to social icons to support various styles
* Save contact when processing a lead from the queue

## October 5, 2020
* Support for border radius and backgrounds in email designer
* Update to button border support and default behavior
* update drag behavior for email designer
* updates for social icons sizing

## October 3, 2020
* Update to search reindexing

## October 2, 2020
* Do not allow set on fullname for contacts in json serialization
* updates for email designer styles
* Expand UDF custom contact fields that are indexable
* Add support for setting background images on email container component

## October 1, 2020
* Remove removeTableIfEmpty from email designer
* Add support for lead reindex queue
* Validate that user has mobile number set to receive notifications in automations
* RhinoFit "Deleted" Contacts not Updating in DailyStory
* Refactor for tag users in bulk
* Weave excludes under 21 from import
