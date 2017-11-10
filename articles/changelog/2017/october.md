{
	title: 'October 2017 Product Update',
	description: 'Product Updates for October 2017'
}
# October 30, 2017
* Fix minor bug with extended field mappings in magic forms.

# October 27, 2017
* Removed unused campaign achievements features
* update Lead Stats job to use new tables for performance improvements
* Improve performance of IP address lookups
* Change Process Leads to call web hook to update lead activity
* Fix bug in URL hash to force to lower case
* Fix contact extended properties to serialize
* Performance improvement to lead dequeue
* Improve performance of salesforce sync and support field mappings

# October 23, 2017
* Updated magic forms to better handle multiple forms on a single page
* Fixed bug in PageInfo that resulted in an empty title
* Fixed bug in link summary report
* Added support for form id in magic forms
* Added new triggered web job for processing lead queue
* Fix bug in web session with page lookup
* Add support for custom lead fields in magic forms
* Add email validation to magic forms

# October 20, 2017
* Big refactor for webstats to improve lookup time and overall performance
* Added job for lead activity updates
* Fix key conflict on ppc campaigns job
* Better logic for ip lookup on web tracking queue processing

# October 17, 2017
* Added support to fetch element id and moved xpath selectors to ds
* Updated some function visibility in Ds javascript library
* Added support for finger print dsid generation for better cross-site support
* Added support for selecting the submit button via post message

# October 15, 2017
* Fixed bug in Web Session report display
* Changed lead detail to use Common formatter for City, Region and Country
* Renamed PPC Click Fraud to just Click Fraud and apply to all links
* Added IpInfo view
* Changed lead page views report to include all leads
* Include IP addresses in link summary report
* Updated/added more unit tests
* Added job for lookup ip addresses
* Fixed bug in lookup ip address for known lead
* Added job for better handling page events from queue
* Better exception handling for web2lead
* Improved performance/behavior of WebTracking
* Fixed bug in clean up job
* Fix bug in auto capitalization
* Added IpInfo class for better ip address management/lookup
* Updated several reports to use async

# October 13, 2017
* More optimistic wire-up for magic forms
* Better IP address tracking/management
* Fix bug in word capitalization when there were multiple spaces
* Fix for handling multiple instances of DailyStory load script
* update Magic Forms to select a single button/input
* Added some info to magic forms to help with debugging

# October 12, 2017
* Add global toggle in user settings for new lead notifications
* Add auto-detect support for Marketo in Magic Forms javascript lib
* Updates fixes for Page Events
* Removed NotificationUser class as part of new lead notifications refactor
* Fix minor bug in redirect logic to prevent fall though
* Better handling of expired tenant js requests to not 404

# October 7, 2017
* Added robots.txt to /ds
* Started automatic event tracking
* Cleaned up some older files

# October 3, 2017
* Added better descriptions and videos when applications have no data
* Fixed bug in Automation Rule on ambiguous match for Int Equals comparison for rules
* Cleanup Contact GetContactAsync method had unused parameter that was no longer needed
* Better exception handling for leads and added GetLeadAsync method
* General refactoring/cleanup on some methods