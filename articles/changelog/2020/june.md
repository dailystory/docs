{
	title: 'June 2020 Product Update',
	description: 'Product Updates for June 2020'
}
# DailyStory Product Updates for June 2020
## June 30, 2020
* don't dispose httpclient after request

## June 29, 2020
* refactor scheduled message to support queues
* add proccess queue job for scheduled messages
* bug with file manager picker - should empty before populating
* set font sizes in popup editor
* remove tooltips

## June 28, 2020
* bugs with popup rending first time
* bugs in campaign graph for empty settings

## June 26, 2020
* bug with uploading svg files to file manager
* update license expiration date behavior
* support svg images

## June 25, 2020
* handle case when queue message is already removed
* throw better exception message when urlhash is not found
* change logic for when dashboard is shown or welcome screen
* bug with setting background in popup

## June 24, 2020
* send a single text message
* add conversational stub for threaded sms messages
* ux for search
* refactor distance calculations to allow for 0
* return null when filter is not found
* handle case when results from search is null
* refactor how route lead handles account and subaccount
* refactor contacts to handle how throws when not found; and find contact by precedence
* bug with how preferences were set for mobile tenants
* don't throw just skip bulk upsert records missing email or mobile phone

## June 23, 2020
* code review and update paths for lead api
* reply address wouldn't save if no senders
* ranged filters are inclusive
* bug with opt out error message other than email
* don't set Lighthouse name and email
* turn mobile/desktop on and off
* delete message earlier and hold in queue for 2 horus
* refactor text messages to use personalized class for handlebars
* bug wth setting text in tinymce in web form
* updates to send single message
* allow logging of messages with a 0 id for send single
* add support for sms replies to customers

## June 22, 2020
* style updates to designer
* disable pre-flood sending for some accounts
* fix bugs in page designer and add support for asset preferences
* bug when creating new form
* style updates for flex layout and open/close tab
* lock on table update for email urls as is not thread safe
* bug in autopilot name for popups: WhenPopupIsSubmitted
* remove workflow from campaign ux

## June 19, 2020
* update urlhash to allow for query string and fragment
* on merge, make sure contact optout preferences can be updated
* refactor mergeasync and handle mobile phone lookups
* bug plaintext body should get personalization
* new EmailUrl for managing urls to hashed values for link clicking in emails
* refactor how email clicks on links are handled
* refactor event webhooks
* trim settings for user values for urls, etc.
* add new route for email clicks
* remove ip blocking from config for iisexpress support
* refactor designer to include mobile toggle and hide properties
* Dequeue messages for 24 hours
* drag and drop notice for content pages
* text can only be dropped in a column in designer

## June 18, 2020
* bug with personalization variables in plaintext emails
* url helper bug that didn't properly process fragments with &

## June 17, 2020
* update to support running issexpress

## June 16, 2020
* bug with search not returning correct number 
* bug with tags api supporting both patch and post
* add api to return a list of optouts
* updates to popup editor
* handle boolean on contact import for opt out
* handle case when strip api not present
* handle case when contact has mobile phone and no email
* only set user-agent header once in singleton http client

## June 15, 2020
* handle case where salesforce doesn't have an email address

## June 12, 2020
* Stripe API environment key only looked up on demand
* Don't apply utm codes to unsubscribe links
* handle case when get a /ds/ds redirect
* bug in system admin for create tenant path
* remove browser check from main header include
* updates to popups
* add browser checks
* refactor how popup manages displayed content

## June 11, 2020
* change popup radio button behavior in layout selection
* clean up popup CSS
* remove style on layout preview
* Calculate validation hash on domain and path only

## June 10, 2020
* initial check in for anniversary filter in search
* support matching exact domains with Mailgun
* Verify credentials for each sending domain
* fix some ux bugs in content pages
* clean up popup designer javascript
* api to get popup
* convert popup design to load from javascript

## June 9, 2020
* update api to support post and patch
* remove unused color picker
* update browser version check script

## June 8, 2020
* Bug handling identifier fragment in url hash for emails
* more search selector clean up
* updates to system
* better support for multiple sending domains

## June 7, 2020
* Remove search selectors

## June 5, 2020
* improvements to how campaigns get refreshed
* updates for help integration
* modify to allow for custom nav
* Add system authorization claim
* add tenant to audit log
* refactor get tenant
* add files for system admin

## June 4, 2020
* fix over reporting issue with link tracking report
* Update to asset preferences to allow for custom logos
* updates to help links
* update refresh campaigns to only process 100 at a time
* link popup help in designers
* funnel filter by date
* Remove dashboard report code that was slow

## June 2, 2020
* wire up new inline help documentation

## June 1, 2020
* update to use helpdocs
* change tracking code to beacon
