{
	title: 'March 2019 Product Update',
	description: 'Product Updates for March 2019'
}
# DailyStory Product Updates for March 2019
## March 25, 2019
* Bug: calling web job in contact save causes asynchronous operation exception
* Bug: new ip addresses to filter
* Refactor: better exception message in mailgun
* Bug: set date created in exception message
* Bug: check Rot13 before checking valid url
* Bug: additional details can be empty string
* Bug: tenant create alpha check fails with spaces
* Refactor: add HasFilters
* Refactor: csv exports
* Refactor: add exception tracking to admin settings

## March 23, 2019
* Bug: double logging api exceptions
* Refactor: better url handling for bad urls

## March 22, 2019
* Bug: fix link tracking redirect bug
* Refactor: log 404s as events
* Bug: link tracking could cache requests and not log properly
* Refactor: include original url in global web app exception

## March 21, 2019
* Bug: errors in application handled better
* Refactor: add support for logging system events
* Refactor: handle multiple exceptions in same batch
* Bug: reason may not be set in optout
* Refactor: improvements to messages
* Bug: unsubscribe converted to use model

## March 20, 2019
* Refactor: better exception handling in LightningContext
* Refactor: better exception management in data center lookup
* Bug: handle case where we can't determine data center in logger
* Refactor: handle case where dsid needs to be generated
* Refactor: capture mail server code when failure occurs
* Refactor: add comment that date is utc in notification alerts
* Refactor: updated campaign stats to better bulk update
* Refactor: updated lead stats to better bulk update; moved out of leadstats job
* Refactor: better exception management for link tracking
* Refactor: move web request processing to core
* Refactor: capture code in failed emails from mailgun
* Refactor: remove how map file was loaded
* Refactor: search 18 age range
* Refactor: move validation to save event for links
* Bug: don't require stack

## March 19, 2019
* Refactor: update generatewebviewhtml
* Refactor: process contact queue to handle bulk updates
* Refactor: move map file reading into bulkimportcontact as internal
* Bug: mergeasync needs to handle invalid contacts
* Refactor: add callback to pleasewaitoff
* Refactor: move routines out of CMS into common
* Bug: dedup batch contact update
* Refactor: handle multiple domain lookups
* Refactor: clean-up and refactor cms

## March 18, 2019
* Refactor: modify to use ds_integration_sync table
* Refactor: link tracking identifier needs to be public

## March 17, 2019
* Bug: total counts were incorret in Mindbody paging
* Refactor: move logging to diagnostic folder
* Refactor: clean up unused enum exception types
* Bug: ignore full name on json serialization
* Refactor: Contact bulk update
* Remove: contact change status
* Bug: handle addresses with + instead of space
* Refactor: add import from file command line
* Refactor: replace thread sleep with task delay
* Refactor: better exception logging for link tracking
* Refactor: add notification for exceptions
* Bug: \n character should not be removed from whitespace
* Refactor: better error message
* Refactor: better email send logging counts
* Refactor: better exception messages for leads
* Refactor: better exception logging for push and text msg
* Bug: UpdateOrphans disabled
* Bug: Degree37 deferrale type

## March 16, 2019
* Refactor: fix logging bug in Mindbody
* Bug: handle no email set Mindbody

## March 13, 2019
* Add: better exception logging and event logging to MindBody
* Bug: handle client id not set in MindBody api
* Refactor: handle exceptions in ProcessTaskQueue
* Refactor: handle global exceptions

## March 12, 2019
* Add: Exception and EventLog reports
* Refactor: better exception management

## March 11, 2019
* Refactor: add async
* Refactor: check if table exists
* Refactor: remove unused exception status
* Refactor: remove references to data center
* Refactor: GetBirthday returns next birthdate; add internals for testing
* Refactor: internals for testings;updates for unit tests
* Refactor: remove license exceptiontype enum
* Bug: check for min date should occur before timezone offset
* Refactor: add support for last sent date
* Bug: handle nulls when not emails sent; bug with optout counts
* Refactor: count optouts
* Refactor: don't use rewriter for optouturl; fix bad urls
* Bug: handle relative urls
* Refactor: handle bad plaintext html nodes
* Add: NormalizeWhiteSpace routine to remove extra whitespace from string
* Refactor: format mailgun exception logs
* Refactor: add command line options for bulk import
* Refactor: add better global exception logging for unhandled web errors
* Refactor: log any auth exceptions
* Refactor: add contacts column
* Refacctor: ActivitySummaryReport to capture contacts

## March 10, 2019
* Refactor: mark as internal for testing
* Bug: graph fields should not return none
* Refactor: don't recreate queue if already exists

## March 9, 2019
* Refactor: update Google Apis to support customer keys
* Refactor: update contact validation
* Refactor: improve proper case handling
* Refactor: handle multiple table lookups
* Refactor: clean up event web hooks to prevent duplicates
* Removed: old test for jobs

## March 5, 2019
* Bug: avg conversion limits
* Refactor: add api for sending a test message
* Refactor: resize assets in campaign
* Bug: not handling error in api javascript
* Refactor: update sms to use drop down similar to email
* Refactor: updates for degree37 integration
* Refactor: campaign stats for better testing and support for limits on conversion rates
* Refactor: updates for unit tests
* Refactor: changes to text message logging
* Refactor: text message logging and send to contact

## March 2, 2019
* Refactor: address sort order tables

## March 1, 2019
* Bug: copy asset caused preview path to get reused
* Refactor: address formatting for graph done in common
* Refactor: RemoveLineBreaks
* Refactor: fix typo in campaign description