{
	title: 'January 2018 Product Update',
	description: 'Product Updates for January 2017'
}
# January 23, 2018
* Fix bug in email sync retry logic
* Fix bug in date formatting for open report
* Fix bug in month formatting for click through reports
* Added lists member of to contact detail and remove logic
* Added versions for css and js
* Added better timezones to create contact
* Added common countries to create contact
* Set focus on firstname when contact create loads for keyboard tabbing

# January 22, 2018
* Moved google maps into a click through vs showing map on contacts and leads
* Added Organization Page View report
* Fixed bug with Link controller
* Added contact website as an editable field
* Advanced search for contacts
* Started moving date picker javascript to main javascript library
* Fixed bug in Emails when using an email template
* Refactoring and clean up descriptions on several pages
* Fixed bug in how email counts were being done
* Remove return statement in lead stat summary
* Added SyncGmail job
* Updated search to read in campaign details
* Additional tests for jobs and components
* Sync contacts with Salesforce Ids
* Fixed bug in CMS landing pages javascript
* Fixed bug in how date/times were calculated using UTC offsets
* Added date_contact_last_modified timestamp
* Updated email tracking bug to be added before closing </body> tag
* Fixed bug in Activity Item sorting that was happening after item was in cache
* 

# January 17, 2018
* UX improvements to contact view
* Remove from campaign support with confirmation on contact
* Fix reporting/graphs on email campaign summary
* Fix bug with date/time conversions for calculating today's date
* Update Salesforce Contact UX
* Added report link to Email edit view
* Add hover titles for email index view
* Added avatar to lead view
* Removed lead text from lead pager
* Cleaned up Bounce, Click, Open and Email Summary reports
* Better handling for fluid layout

# January 16, 2018
* Add support for avatar lookup
* Add audit contact activity type
* Added SFDC contact lookup

# January 15, 2018
* Add List end point for Contact List
* Added confirmation UX for delete
* More checks for optout, don't add to campaign
* Improved UX for API key management
* Fix bug in delete contact list
* Added Add to list option for workflow
* Added Add to list option for automation
* UX to use lead or contact depending on campaign type
* Initial support for adding notes to contacts
* Fixed bug in link tracking where new links didn't have a preview
* Changed Save Button to use red colors
* Added automation support for Addtolist
* Added timestamp for contact creation since DateCreated is date only
* Added non-async methods to ContactList
* Better error handling for content pages
* Bug in counts for emails opened and clicked (only counting unqiues)
* Bug that overcounted (deleted) contacts
* 
# January 10, 2018
* IFrame slug type for CMS content

# January 9, 2018
* Don't send new lead notifications for leads created throught UX
* Added Zapier to integrations pages
* Refactored Campaign Header to support Campaign in Views
* Clarify use of Contact or Lead
* Updated dates to 2018
* Change clean up job to run daily
* Tracking URLs should handle mailto links in emails
* Added some trim on URLs for tracking links
* Force notification to use DailyStory.com email server
* Updates/refactor conversion rate report
* Better handling of failed transactions for WebTrackQueue

# January 8, 2018
* Add UX to indicate if campaign is active, deleted or paused
* Fixed bug in controller action to update credit card
