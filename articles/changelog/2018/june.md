{
	title: 'June 2018 Product Update',
	description: 'Product Updates for June 2018'
}
# DailyStory Product Updates for June 2018
## June 30, 2018
* Update: Advanced search to handle various error conditions in filters
* Feature: Added search error hander
* Bug: Mailgun could show as tenantdefined in some cases when it wasn't
* Bug: TLS 1.2 for LInkedIn Api requests
* Bug: bug in javascript handler for search
* Bug: better test experience for popups
* Bug: fix regression with search button 

## June 29, 2018
* Refactor: pass tenant instead of id
* Bug: fixed serialization bug in ActivityTableEntity
* Refactor: cache on tenantuid
* Feature: add age calculation to common and remove from contact
* Refactor: Separated SegmentList from Segment
* Refactor: Connection provider
* Refactor: add coerece bool to graph field
* Feature: OpenStreetMap get first found location
* Feature: added support for bool and double types to graph field
* Feature: added fields to Activity Type
* Bug: issues with lead pages checking wrong page size in some cases
* Refactor: Lightning Context double-checks tenant uid
* Refactor: logging
* Refactor: update packages
* Refactor: ContactDocument added more types and age
* Refactor: Search Filter on Contact Document and parse querystring
* Refactor: integrations datamanager, move all settings to azure tables
* Refactor: start queue updates for scale on email
* Refactor: UX for advanced search
* Refactor: white label

## June 25, 2018
* Feature: enable white label tenants to show their logo in UX

## June 24, 2018
* Bug: Strip re-captcha on form submit
* Refactor: LeadQueueItem
* Refactor: DailyDigest notification sends 204 if there are no leads or contacts
* Refactor: Ensure web stats reports returns data
* Allow access control origin on about
* Refactor: admin level reset password
* Bug: daily digest content was getting trimmed
* Bug: social media account had bug with how updates were run

## June 23, 2018
* Bug: domain preview with custom domains built links incorrectly.
* Refactor: Force TLS 1.2 on api requests
* Refactor: Web Form lookup table
* Refactor: integration table lookups
* Bug: content pages failed on pages with an id of less than 1
* Added cryptography class
* Refactor: connection provider
* Refactor: Link Tracking look up table
* Refactor: safe cache keys across tenants

## June 22, 2018
* Refactor: guard rails around account / user management
* Refactor: convert system account settings to encrypted
* Refactor: better UX for add/remove user and guard rails.
* Refactor: better domain lookup support

## June 21, 2018
* Refactor: better exceptions for notifications
* Refactor: trigger web jobs.
* Refactor: fix webstats build warnings
* Refactor: fix leadstats build warnings
* Refactor: updates to DailyDigest
* Refactor: fix update ip address build warnings
* Refactor: updated project build paths
* Bug: redir string could be empty
* Bug: web hook for jobs

## June 20, 2018
* Refactor: use environment variables for system lookups.
* Refactor: better construction of app path
* Created powershell scripts for changing local environment flags
* Updated: updated how integrations handle connection lookups
* Updated: mailgun error message
* Bug: campaign account owner UID not set
* Bug: better app path rewrite for different data center
* Bug: non-breaking, but fixed null when creating new campaign in ux-campaign-selector
* Refactor: updated some form styles
* Bind content gallery to dc-1
* Refactor: fix some old cms connection strings
* Update: style enhancement on send test email
* Bug: fix path dependency in image store

## June 19, 2018
* Bug: Support reverse link lookup to data center for tracking links
* Refactor: Add ds_tenant_datacenter lookup table
* Refactor: Remove use of tenant id for building connection strings
* Bug: Css update for field
* Bug: update terms of service links
* Bug: update connection provider environment variable

## June 18, 2018
* Bug: fix mac UX bug in email editor
* Refactor: move visit alerts javascript to bundles
* Refactor: move field input support to a global css
* Refactor: refactor pass on page triggers
* Bug: ensure bad queue items don't over notify for leads
* Refactor: add support for Common Remove Non Alphas for Field Graph
* Refactor: add some check conditions for handlebars
* Refactor: page triggers populates Name value of target

## June 17, 2018
* Refactor: continued split login into system tables
* Upgrade tinymce

## June 16, 2018
* Refactor: split login into system tables

## June 15, 2018
* Update: remove data center dependency from CampaignStats
* Update: remove data center dependency from CampaignWorkflows
* Update: remove data center dependency from LeadStats
* Update: remove data center dependency from ProcesEmailClickOpenQueue
* Update: remove data center dependency from ProcessLinkTrackingQueue
* Update: remove data center dependency from WebTrackQueueItem
* Update: update libraries and remove data center dependency from RunAutomations
* Update: update libraries and remove data center dependency from RunCleanup
* Update: update libraries and remove data center dependency from RunMaintenance
* Update: update libraries from SyncMailgun
* Update: update libraries from SyncSalesforce
* Update: update libraries and remove data center dependency from WebStats
* Update: update libraries from UpdateAccountScores
* Update: update job tests
* Bug fix on HostInfo
* Update unit tests
* Update: UX changes to CSS
* Refactor: Remove dead API in Campaign
* Bug: Implement campaign add from search
* Refactor: update packages
* Refactor: text message updates with better messages
* Update: update TinyMCE
* Update: error message for bad url in track code tester
* Update: added support for changing Lead text with site terms
* Refactor: update to contact UX
* Refactor: better UX on contract graph
* Update: auto-set the email and mobile number for test messages
* Refactor: text clean up
* Update library packages for web

## June 12, 2018
* Update: import contact to kick off contact queue
* Update: OpenStreetMap tests
* Added: ContentEmailGallery
* Added: Support for email creation from gallery id
* Bug: bug in magic form looking for wrong field id
* Refactor: UX work on segments
* Added: preview email for Gallery

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