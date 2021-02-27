# DailyStory Product Updates for February 2021
## February 27, 2021
* Remove select all option on segment bulk edit

## February 26, 2021
* Text keyword into campaign counts as a double opt-in
* Add text message optout report
* Convert segments to use separate js file
* Bug with archive link
* Add bulk archive and delete to segments
* Add ability to bulk edit campaigns
* Campaign archive links should go to campaign edit
* Support bulk pause for segments

## February 25, 2021
* Additional dns-prefetch and preconnect hints for fontawesome
* Leave drop down open to allow multi-select for campaign and scheduler
* Sms index view was set to return messages with any status
* Bug with email api path missing v1 and add support for campaigns
* Delivered display in activity list missing
* Update email and sms send single to send to lead in campaign
* Refactor to allow for istransactional messages
* Convert SentTestAsync to SendAsync to handle single lead sends
* Trigger an automation when assigned a task
* Support trigger when assigned task in automation triggers
* Better error message when lead isn't in campaign
* Refactor email API controller name
* Update to send email / sms single to require lead to be in campaign
* Better logging for sms opt in
* Edits to optin and optout messages for text messaging
* add JOIN as opt in keyword for SMS

## February 24, 2021
* Remove workflow id column dependency
* Performance improvement to email detail reporting
* Add dns-prefetch and preconnect hints

## February 23, 2021
* Allow mailto as a url in validation
* Special case URL hashing for mailto

## February 12, 2021
* Add pre-built fields to methods

## February 11, 2021
* Update to create edit with sections, e.g. mindbody
* Allow for meta name, description and social image to be set for web forms
* Deduplicate works in batch sets of 500
* Typed properties for web form meta fields

## February 10, 2021
* Enable segment building message to be hidden
* Email summary report includes first and last name in separate columns
* Segment export for automation must include name and description
* Set a name for the segment if not specified in automation import
* IsNew check on segment should use UTC date

## February 9, 2021
* Add image picker to text content in web forms
* URL decode search text when using search to add to a static segment
* Sort pick list values in contact detail alphabetically

## February 8, 2021
* Ensure that search string can't contain ?s=
* Bug with formatting of email delivery on failure for activity

## February 5, 2021
* Don't show is segment ready if segment is not dynamic

## February 3, 2021
* Scheduler is expanded by default

## February 2, 2021
* Allow divider to be dropped into email sections
* Convert export contacts task to use ContactEocument export
* Add support for refresh donor by donor id

## February 1, 2021
* Pop Up not working on a DailyStory landing page
* BulkImportContacts missing from WebJob enum
* Log activities better in bulk import webjob
* Update contact activity to use moment for date times
* Convert activity timeline on contact to use javascript
* WebActivity should return URL and title
* Limit contact activity to 25 records
* Custom field picklists should sort alphabetically
* Contact export should include all fields
* Add support to sync a single user in telligent
* Add on demand sync support for Telligent
* Mindbody and Telligent sync clear contact cache
* Add support for social urls as extended profile fields
* Add sync support for degree37/bbcs
