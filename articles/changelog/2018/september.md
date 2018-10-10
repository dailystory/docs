{
	title: 'September 2018 Product Update',
	description: 'Product Updates for September 2018'
}
# DailyStory Product Updates for September 2018
## September 29, 2018
* Refactor: Add Get Set to safely modify ExtendedProperties

## September 28, 2018
* Bug: change how api base set claim
* Bug: pageindex is zero the HasMoreResults always returns true

## September 27, 2018
* Add Azure functions to source control
* Remove: CleanUp job; replaced with functions
* Refactor: enable tenant look ups without cache
* Bug: add user to tenant (sub account) was broken due to cache bug
* Refactor: Consolidate system email into system database
* Bug: 500 error when updating contact profile graph
* Bug: Magic Forms should only work on pages running DS
* Refactor: graph field to save with tenant

## September 26, 2018
* Feature: Implement ContactCanManage and ContactCanView role checks in controllers and APIs
* Feature: Implement ContactCanManage and ContactCanView role checks in controllers and APIs
* Refactor: remove SegmentCanView claim
* Bug: show error message in contact save
* Refactor: GetTenantForUserAsync
* Bug: switch account to switch the whitelabel domain
* Bug: Subscribe to DailyStory newsletter should not add people to MC list
* Bug: Favicon needs to be white labeled
* Bug: Permission error message on save isn't shown.
* Refactor: validate user prior to saving
* Feature: add urlhash lookup to content page

## September 25, 2018
* Bug: check if account owner uid is set
* Refactor: better error messages for invalid emails
* Bug: dequeue contact job could loop endlessly
* Refactor: make checkclaims static
* Refactor: add checks for content claims

## September 24, 2018
* Feature: Add support for page designer form

## September 22, 2018
* Bug: designer could inject external css links into page body
* Refactor: style updates on import and magic forms
* Bug: white label Twilio error message
* Refactor: updates to email and send to campaign

## September 21, 2018
* Refactor: exception handling for email click
* Refactor: add WhiteLabelName merge tag
* Bug: A campaign that has sent email, but has not had any opens reports
* Bug: Notifications should be sent from email domain when whitelabeled
* Bug: Notifications must be whitelabeled
* Bug: System emails need to be white labeled
* Bug: Newletter for DailyStory and option in user preferences
* Bug: Default tenant setting not persisting after saving
* Bug: error trying to remove user from tenant
* Bug: error with user being removed from tenant checking if was tenant owner
* Refactor: add argument exception checks to Lead
* Refactor: add argument exception checks to PageInfo
* Bug: clear cache on save; white label forgot password
* Refactor: Add WhiteLabel property to tenant
* Feature: Add support for dynamic segments
* Refactor: set a type for imported segments

## September 19, 2018
* Bug: graph field couldn't be id'd as lead field
* Bug: admin shouldn't show tracking tag for non admins
* Bug: manage graph wasn't showing delete icon

## September 18, 2018
* Bug: whitelabel failed login doesn't go to whitelabel page
* Bug: designer could attempt to access null head
* Bug: whitelabel text
* Bug: css in edit html can be null
* Bug: show welcome on home not whitelabeled
* Bug: handle exceptions in non-unique slugs
* Bug: ensure import of CSV handles exceptions
* Feature: updates to v2 editors
* Refactor: handle save states for content pages
* Refactor: add error message type 
* Bug: saving rulesets new json
* Bug: welcome screen

## September 16, 2018
* Bug: contract api did not reset stream before reading
* Refactor: lookup tenant from system
* Refactor: add user look up by uid and tenant
* Refactor: improvements to designers
* Feature: create edit pages v2
* Refactor: users enable managing preferences

## September 13, 2018
* Refactor: Updates to resource strings
* Refactor: always allow Administrative role
* Refactor: Email summary object
* Feature: role user count and check if name is used
* Refactor: UX for CSS field inputs
* Refactor: API auth base to claims; new CheckClaims for code
* Refactor: use checkclaims and normalize role checks
* Refactor: Add footer section to designer
* Refactor: better route management for APIs
* Refactor: UX for contact import

## September 12, 2018
* Refactor: Set the name of the segment that is imported to.
* Refactor: validate on user lookup
* Refactor: Added check for is user in tenant
* Refactor: better error handling and manage administrative claims for roles
* Refactor: Button for designer
* Refactor: Error message changed to white background for image
* Feature: added claims check to Campaign controller
* Feature: added segment name to map file
* Feature: Roles UX management
* Bug: arrow not shown in designer
* Feature: Add roles to control what is shown in layouts
* Refactor: javascript updates to handle errors properly
* Feature: added claims check to Segment controller

## September 6, 2018
* Refactor: button for button in designer
* Bug: fix issue with overflow causing seletor to get offset
* Refactor: better message when browser is too small
* Bug: ensure only css files are loaded into editor
* Refactor: Move some calls to functions; ensure bootstrap loaded

## September 4, 2018
* Feature: HotMetal designer and editor for content pages 
* Refactor: update to list of published role claims
* Refactor: update job package files to latest versions
* Test: updated unit tests
* Refactor: continue roles updates
* Refactor: message ux for in system messages
* Refactor: update email views
* bug: prevent small screens in designer