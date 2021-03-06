# DailyStory Product Updates for September 2020
## September 30, 2020
* Bug with async fetch in workflow
* Add UpdateMobilePhoneAsync similar to update email
* Randomize dequeue for sms status
* Move contact segment reindexing to separate queue
* Move contact campaign reindexing to separate queue
* Move contact tag reindexing to separate queue
* Move contact email opens and clicks reindexing to separate queue
* Move contact reindexing to separate queue
* Text message contact reindexing
* add support for custom fonts in email designer
* add send test from email designer
* add class for images to support full width on mobile
* Check to ensure that the user has a valid phone for mobile notifications in automations

## September 29, 2020
* updates to email designer v2
* Bugs with undo of fetch async
* Add support for partial contact indexing
* Bug with how full name is handled in search
* unwind email designer v2

## September 28, 2020
* Initial check-in for email designer v2

## September 25, 2020
* Add conditions for can receive email or sms
* Mobile phone validation should fail if the number is less than 10 digits
* Add conditions for can receive push notifications
* Add UX for autopilot for receive email, sms or push
* Updates to support RhinoFit contacts with mobile number
* Bug with search export including reserved token

## September 24, 2020
* Enable setting borders in email designer sections
* Add additional email templates
* Bug with image rendering height on email images
* Update email status change needs to update contact properties
* Updates to RSS email component
* parse RSS for images in email

## September 23, 2020
* Import email from URL
* Updates to add in support for pre-built email templates

## September 22, 2020
* Iteration on email experiments
* Handle license exception bug for text messages in automations
* Bug with lost conversion calculation

## September 21, 2020
* More segment details on recipients for SMS
* Export large segments in background task
* Update segment stats with email and sms enabled
* Add support for deleting experiments
* Add support for AMP emails
* Bug with load data order in automations

## September 18, 2020
* Convert search to a continuous job
* Bug with how bad / invalid email addresses were handled in Neverbounce
* Bug with how birthday was handled in RhinoFit sync
* Bug Value cannot be null or empty.  Parameter name: linkText
* Bug An item with the same key has already been added.
* Bug import should validate dsid and mobile phone too
* Handle email format exception from NeverBounce
* Bug with Weave allowing duplicate customer ids across locations
* Redirect to login on account not found
* Bug check for null string on name in file manager

## September 17, 2020
* Bug with copy popup not setting id correctly
* Add 2 and 3 col image layouts
* Update WebTracking to use CosmosDB
* Bug scheduler should specify message send type
* More updates on email experiments

## September 16, 2020
* Add support for scheduling a multivariate email
* Refactor email experiments
* Support sending an email experiment
* Bug with js minification

## September 15, 2020
* Add support for contact merge
* Bug with offset height in page designer
* Add help article to merge contacts
* Bugs with system redirect on create tenant
* Bug with deserializing fullname
* Change throttle on text messages
* Run blocks validation on update for automation
* Consolidate text message reply handling into single condition
* Link to replies from menu

## September 14, 2020
* Inline menus need to be consistent
* Update links to reports in camapign assets for magic forms and web forms
* Updates to search form description, disable auto-complete on dates and add first engaged
* Update ContactDocument to support DataFirstSeen
* Bug need to handle DataFirstSeen as null in search
* Automation for when removed from or added to segment 
* Remove button location in automation is in the wrong "flow" of the user activity
* Added anniversary segment to templates
* Ability to Add Email using a template from within a Campaign

## September 12, 2020
* Bug with v1 path reference
* Allow font selection and size in email designer
* Refactor email designer into component files

## September 11, 2020
* bug with task association api
* Add support for RSS driven emails
* add RssEmail into handle bars compile for emails

## September 10, 2020
* Bug with callback on file manager - needs to get reset
* More refactor on popups
* Refactor invite to be more personal
* Add function to check if a dsid guid is already provisioned
* Refactor create edit ux

## September 9, 2020
* Inline menus need to be consistent
* Main nav documentation link opens full docs
* Invitation javascript has bugs with setting the password - should be a separate Js file
* Text Automation has issue with duplicate contact records sharing the same mobile number
* Refactor and update funnels
* Merged in design consistency branch
* Change sequence of when ace editor is initialized for the popup
* update menu consistency for emails

## September 8, 2020
* Bug Paused campaign has wrong message
* Add support for dedicated function to GetFullname
* Bug with reports not rendering without fullname
* Improvements to performance of add segment to campaign
* Updates to HTML editor and start support for AMP
* Convert to use Tiny MCE toolbar for consistency

## September 5, 2020
* Status queue items expire after 72 hours
* default SMS messages to delivered

## September 4, 2020
* Add support for custom button position for popups
* Updates for designer consistency across editors
* Add support for renaming files and folders in file manager
* Bug Insert Image not working in Email Template Edit screen
* Update Email HTML Editor for consistency
* Bug new contact save with empty full name over writes valid name
* Inline menus need to be consistent

## September 3, 2020
* Updates for responsive UX
* Remove old log redirect url
* Allow for ranged searchs of 0 to include null when only using from
* Add support or formatting friendly location
* Refactor GetNewLeads to GetInboundLeads
* New apis for leads
* Improve performance of home page
* bug when checking search array item for space
* handle unprocess text messages that are returned as status sent

## September 2, 2020
* Increase weight for bad url and some words in sms scoring tool
* refactor for create edit funnels
* Improvement to focus screen ux
* Add support for medical license expiration in Weave sync
* Better experience with highlighting help docs

## September 1, 2020
* Scheduler deleting scheduled items when edited
* Begin refactor of account functionality
* Refactor of contact vNext UX
* Allow fullname on contact to be serialized
* Updates to contact activity report
