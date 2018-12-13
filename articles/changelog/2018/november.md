{
	title: 'November 2018 Product Update',
	description: 'Product Updates for November 2018'
}
# DailyStory Product Updates for November 2018
## November 30, 2018
* Refactor: move css styles to file
* Bug: last segment or campaign in a contact should remove the card
* Bug: cache wasn't consistently cleared for add/remove segments
* Add: Contact Preferences to better manage how contacts optin and optout
* Refactor: make table cell clickable for leads, contacts and campaigns
* Refactor: one click edit from contact list
* Refactor: merged in screen-edits branch for UX updates
* Bug: body merge tags handled incorrectly in notifications
* Refactor: check for do not contact when sending text msg

## November 29, 2018
* Refactor: updates for new optin and do not contact options
* Merge: merged in new optin management preferences and screen

## November 28, 2018
* Refactor: Updated unit tests and sync on sales for MindBody
* Refactor: more updates to social media posts
* Refactor: Enable popups to capture mobile phone number
* Bug: don't return import segments on static request
* Refactor: add mobile phone in lead queue
* Refactor: updates to social media
* Refactor: add syncsocialmedia to jobs list webhooks
* Refactor: show form modal in popup editor to assist user with validation

## November 27, 2018
* Refactor: add indexed properties to exported CSV
* Refactor: make non async get segment thread safe
* Refactor: change import to use batch updates
* Bug: delivery stats calculated incorrectly
* Refactor: include mobile phone in export of leads to csv
* Bug: can't have multiple pagers
* Refactor: update to preferences UX
* Refactor: [MindBody] remove SetContactStatus
* Refactor: Updates to Social Media

## November 25, 2018
* Bug: workaround for deserialization of SearchFilter json
* Refactor: rename delete tenant
* Bug: check in tasks of deserialized search filter should check for tostring
* Bug: random filters object in Contacts
* Refactor: rename members to contacts in segments
* Refator: refresh the segment if all items are removed from a view

## November 23, 2018
* Refactor: handle task based addition of contacts to segments
* Bug: reconcile searched based add vs full update
* Refactor: continue adding support for new do not contact
* Refactor: add contacts to segments task
* Refactor: better navigation in error messages
* Bug: white label redirect bug on invitation
* Bug: handle Ds paths that aren't qualified URLs and add http

## November 21, 2018
* Bug: paging could break in contacts with search results
* Bug: column not hidden in media query for emails
* Bug: contact fullname set/get may not get read correctly
* Bug: contact fullname set/get may not get read correctly
* Bug: only return active contacts in dynamic search
* Refactor: allow updates of a specific segment

## November 20, 2018
* Feature: add support for SaleService in MindBody integration
* Bug: role check for segment can manage had typo
* Refactor: usernames in roles clickable
* Feature: get client services into contact array (MindBody integration)
* Refactor: update installer to support new MindBody field
* Bug: bug in add users

## November 19, 2018
* Bug: paging support in segments
* Refactor: add segmentcreateeditmodel
* Refactor: segments add/remove in edit campaign
* Refactor: allow filename to be specified/persisted for import
* Refactor: add debug type with queues
* Bug: handle cases where message doesn't exist
* Refactor: Add/Remove segments through campaigns

## November 17, 2018
* Bug: utm links in emails not whitelabeled
* Refactor: performance improvement for rebuilding dynamic segments
* Refactor: send notifications when import completes
* Feature: Segments GetSegmentsForCampaignAsync

## November 16, 2018
* Refactor: add trace to jobs and remove dead wood
* Refactor: performance improvements for last seen calculations
* Refactor: Notifications for bulk import
* Refactor: gracefully handle malformed segment search queries
* Refactor: performance improvement for campaign stats calculations
* Bug: fix flicker in segment load

## November 15, 2018
* Bug: handle license exceptions in graph fields API
* Refactor: Update lead graph javascript
* Bug: add trim on validator
* Refactor: ManageGraph to support adding indexes in UX
* Refactor: better batch processing for delete contact
* Bug: contact search in segments broken; sql error
* Refactor: GraphField
* Refactor: add license check api for search indexes
* Refactor: tidied up lead notifications subject
* Refactor: batch update for ContactDocument
* Refactor: update for user defined lead fields

## November 14, 2018
* Refactor: reset user status after login
* Refactor: handle bad search filters for custom ranged dates
* Refactor: improve search job and move logic into core
* Refactor: add support for reinvite to join and clean up
* Refactor: add support for reset inivitation
* Refactor: set login date for new users to sql min val
* Refactor: update admin users to re-invite users
* Refactor: subtle buttons in campaigns
* Refactor: exports support extended properties

## November 13, 2018
* Refactor: style updates for segments to use tables
* Bug: phone formatting in contact
* Refactor: friendly datetime with no user offset
* Refactor: improve performance and calc up date last seen
* Refactor: add support for count in segment
* Refactor: move queue debug mode to compiler directive
* Refactor: async for campaign action selector and exclude dynamic segments
* Bug: get dsids should use SearchModel.All
* Bug: handle deletes in search selector

## November 12, 2018
* Refactor: Updates to LeadPageView report
* Refactor: BaseSendDateTimeRule
* Bug: handle multilple s= in dynamic segment as OR
* Refactor: return total views in page view report
* Refactor: add delete logic for campaigns
* Refactor: updates segements UX
* Bug: bug in how Date is calculated in Safari
* Bug: schedule wrapper not being shown in emails
* Refactor: style segments
* Refactor: better campaign navigation in email
* Refactor: convert rule model to async

## November 8, 2018
* Refactor: improve search index performance
* Refactor: Add support for Contact Activity
* Refactor: segments

## November 7, 2018
* Refactor: CSS for edit on magic forms
* Refactor: quick buttons on campaign
* Bug: white label on SMS
* Refactor: return full tenant
* Refactor: performance enhancements to contact import

## November 6, 2018
* Refactor: clean up OwnerId in Account
* Feature: updates to Account
* Refactor: fix build warning
* Refactor: fix GetTenant for user
* Refactor: Performance improvements for bulk import
* Bug: handle whitelabel redirect on password reset
* Refactor: lead stats job
* Refactor: move ScheduledMessage send to Task job
* Refactor: delete contacts in segments that no longer match search
* Refactor: remove exception type lead not found
* Refactor: add wrapper method for send if ready
* Bug: email send handle lead not found
* Bug: remove lead contacted on queue send

## November 5, 2018
* Bug: Paging through contacts breaks with a search filter
* Refactor: use flags for common status filtering
* Bug: cloning multiple campaigns couldn't convert from int[]
* Bug: token cache key lookup
* Feature: add support for segments on leads and emails

## November 4, 2018
* Bug: AND keyword breaks in advanced search
* Bug: don't allow AND or OR leading searches

## November 1, 2018
* Feature: campaign cloning
* Refactor: more helpful search error message
* Refactor: update message template
* Bug: change password showed wrong notification message state
* Refactor: added callback on confetti
* Refactor: added invalid to message type
* Refactor: support for clone batch subaccounts
* Bug: search cannot start with * or ?
