# DailyStory Product Updates for January 2021
## January 30, 2021
* Add api end point to run SyncMindBody for a given client id
* Refactor trigger web jobs and add support for calling syncmindbody to sync a client id

## January 29, 2021
* Updates to deduplicate logic to support mobile phone
* Refactor condition wait time and process specific url clicks for emails
* If a step fails, should be logged as failure not complete
* Remove GetDsidsChunkedAsync
* Add groupname to api graph output
* Disply custom section for Mindbody information in profile
* Add support for custom fields types in contact detail
* Custom contact fields should use sections, e.g. "Salesforce" vs listing all together

## January 28, 2021
* Trigger automation job
* Updates to how contact auto-merge occurs
* Add task for when RSS feed changes
* If min updates is less than 1 set to 1 for RSS
* Refactor contact merge
* Add automation condition HasSubmittedWebForm
* Add condition to automation for HasSubmittedWebFormAsync
* Add quick create link for automations
* Send single text wasn't shortening link
* Bad null check on automation export
* Handle click tracking for double opt in email links
* Bug with image width for emails when set to a fixed width
* Sory automations by last updated by default
* Condition for new contact need to use timestamp contact created
* Trigger automation to run when conditions are met

## January 27, 2021
* Handle drag position when screen is scrolled horizontally
* Handle enable/disable if automation is invalid in a campaign
* Add shortcut link to CREATE NEW.. SMS or Email from their list screens
* Add Evaluate text message reply
* One off email send giving an API error
* Add support for auto deduplicate tools

## January 26, 2021
* Campaign has sms activity and message should not be shown for inactivity
* bug in workflow is valid
* Bug that could cause wrong lead id to trigger when there are duplicates
* Text message should trigger condition checks on message reply
* Add condition handler for text message replies
* HIde properties when drag to delete in automation
* Larger canvas size for automation designer

## January 25, 2021
* Bool data types in for contact custom fields should pass a querystring parameter
* Audit log for send message should use message id not schedule id
* Automations need "Draft" mode
* Add MindBody Field NUMBER OF VISITS to sync

## January 22, 2021
* Swap label and placeholder on web form designer
* Closing web form designer side bar should hide trash

## January 21, 2021
* Filter out spammy looking leads
* Double opt-in should record IP address
* Remove UpdateSearch webhook, no longer needed and refactor webhook enum

## January 20, 2021
* Updates to autopilot to support importing new export format
* Remove legacy autopilot export/import
* Update AutomationExport to support tags
* Handle encoded urls for automation url import
* Decode url in url helper
* include doc links in white labeled instances
* Possible bug with create segment in system
* Support please wait when segment is new and building

## January 19, 2021
* Bug with how tenant id was set in magic forms
* Export automation includes all automation assets

## January 18, 2021
* Update placeholder color and positioning for search
* Refactor magic form javascript and support click to open
* Bug in SendEmailNotification item name
* Preview and edit email from within automation
* Bug with check waittime vs hours
* Edit text message from within automation
* Preview and edit popup from within automation
* Preview and edit magic and web forms from within automation
* View and edit segments from within automation
* Edit push notifications from within automation
* View and edit campaigns from within automation

## January 17, 2021
* Enable Mindbody integration to support multiple locations in a single instance
* Update Mindbody installer to handle multiple site ids
* Change Mindbody integration configuration for retrieving activation code
* Change more option in link tracking to be consistent
* Support for tenant with multiple site ids in Mindbody
* Update pick list fields should allow for name to be included

## January 15, 2021
* Reports should still be available for non-active assets
* Trim inputs for Twilio integration to remove extra spaces
* Text message with image url shouldn't require text
* Handle all caps warning message in deliverability tool
* Update magic form builder to better work with form ids
* change score weighting for all caps in text messages

## January 14, 2021
* Remove padding on th flex for mobile view of emails

## January 12, 2021
* Use of a start keyword counts as a double opt-in for sms
* Refactor experiment a/b test when winner is selected
* Update batch handling of received message id checks on leads
* Updates to scheduler to handle a/b test emails
* Bug setting campaign id in breadcrumb path
* Refactor a/b tests for emails

## January 11, 2021
* Use change event and not keyup in designer
* Add support for Is contact new? condition
* Add support for for double opt in management in preferences
* Add support for *|DOUBLE_OPTIN|* merge tag in emails
* Add support for double optin routes and confirmation screen
* Add email double opt-in widget to automation and automation templates
* Enable weave selective sync
* Merge A/B test variants

## January 10, 2021
* Convert events to use change vs keydown for right-click paste

## January 9, 2021
* name changes of text widget for consistency
* Enable editing of HTML of the text / html widget
* updates to rss email template

## January 8, 2021
* bug with re-building a url wth querystring
* Manage fields shouldn't change sort order when a field is updates
* Refactor CheckIfAlreadyRecievedMessage to allow list of ids
* add scheduled message type for SendEmailExperimentResult
* Support scheduling the test winner
* Remove check on recipient count in UX for a/b test
* Email methods for handling a/b test send logic

## January 7, 2021
* Add link on Bounced Report in DS to HelpDocs article
* Ability to exclude segments/lists when building dynamic searches/segments
* Duplicates in opt-out report
* Undefined status changes in contact log
* Bug with handling ds_rid and setting redirect url
* Convert LinkTracking url builder to use Url Helper's querystring methods

## January 6, 2021
* Don't spell check SMS editing area
* Add "Date Sent" column to email delivered report
* update copyright to 2021
* Multi-field select on contact edit isn't saving
* Pick list values should be shown when available
* Update email 2 column widget to support placeholders
* Value shouldn't be required in pick list to be saved
* Standardize column icons and names in email editor
* Bug with handling leap year birthdays

## January 5, 2021
* Bug in editing or deleting email template
* Bug when try to create a new contact record

## January 4, 2021
* bug with media urls in text messages

## January 2, 2021
* Comment out invalid sending domain

## January 1, 2021
* Updates to landing page designer
