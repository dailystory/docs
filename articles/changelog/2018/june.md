{
	title: 'June 2018 Product Update',
	description: 'Product Updates for June 2018'
}
# DailyStory Product Updates for June 2018
## June 10, 2018
* Refactor: update geo parsing
* Refactor: add support for filters 
* Updated: added search option to segments
* Refactor: rename Import to ImportContact
* Refactor: added ImportDataSet to handle record counts
* Refactor: updated import profile to support ImportDataSet
* Added: OpenStreetMap for geo lookup
* Added: OpenStreetMapPlace
* Updated: added caching to graph field lookups
* Refactor: set types on Contact document UDF fields
* Added: validation check for geo codes
* Updated: Bulk import 
* Bug: fixed bug to set zindex of animation icon above modal
* Updated: converted controllers to use ImportDataSet
* Updated: added support for find location
* Updated: SegmentController to support filters
* Updated: search support in contact.js
* Updated: capture search query value in segments
* Updated: advanced search uses hidden lat/lon
* Updated: contactimport.cshtml

## June 7, 2018
* Updated Azure search libraries
* Refactor: css updates
* Added: support for geo spatial searches
* Refactor: some clean up on view naming
* Refactor: contact edit javascript
* Update: contact search javascript
* Update: lead and lead-edit javascript
* Refactor: twiddled the upload/download icons
* Refactor: updated contact table with new search options
* Added: new methods to common for dealing with lat and long conversions
* Added: support for gender, date of birth and age in contact
* 
## June 6, 2018
* Added: material CSS for radio buttons
* Bug: updated color to form-controls to be darker to pop better
* Refactor: multiple CSS updates/improvements
* Refactor: global rename from List to Segment
* Added: support import of gallery page as template
* Refactor: changes to social media controller to return filtered lists of scheduled or published
* Added: Graph fields to Contact
* Bug: Contact List table was not using material checkbox
* Bug: Contact table was not using material checkbox
* Added: option to manage contact graph fields
* Added: metric to social accounts
* Refactor: minor updates to Web Form
* Bug: Fix bug in how date offsets calculated in social media job
* Feature: Add support for user defined types in search

## June 3, 2018
* Updates: Updates for Facebook, Twitter and LinkedIn integration
* Refactor: add support for ICampaignAsset to ContentPage
* Refactor: small update to Email
* Added: ContentPageGallery, GalleryTypeEnum and other Gallery features
* Refactor: removed TID, CID, and FID from LeadQueueItem
* Added: updates to social media accounts
* Added: social media account summary report
* Update: Social media channel and account
* Update: added more bundled javascript and css files
* Refactor: small CSS update/adjustments
* Refactor: converted popup to async
* Update: added support for Facebook in oAuth app flow
* Refactor: incremental update to content pages
* Refactor: update to prevent switch from redirecting to a identity request
* Bug: Email API List was broken
* Refactor: popup javascript and editors
* Refactor: convert "my accounts" to "sub accounts"
* Refactor: add design time support for page editor

## June 2, 2018
* Bug: content pages from CMS should only serve active pages
* Bug: web form could not find dsid on first request in some cases