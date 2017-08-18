{
	title: 'August 2017 Product Update',
	description: 'Product Updates for August 2017'
}
#August 18, 2017
* Added Export for PPC Search Keyword Summary Report
* Added drill down / detail report for PPC Search Keyword Report
* Performance improvements to PPC search reports
* WebTrackingCallback detects item type from url
* Remove json serialization from slide form
* Refactor PayPerClick link tracking
* Refactored date first seen, last seen and contacted
* Added default to BodyNoTemplate for emails
* Clean up and refactor LInkTracking
* Added tests for ReportBase, PayPerClick, PPC Report
* Abstracted Ds Json rendering to separate class
* Fix bug with date last contacted

#August 16, 2017

* Update for chat to support mobile; s-ton of work over the past week.
* Converted DailyStory scripts to use bundles and split-up respective files.

#August 10, 2017

* DailyStory chat alpha

#August 8, 2017

* Improvements to redirect handling
* Improvements to paid search and link tracking

#August 5, 2017

* Overhaul of DS script for both popups and slide form
* Update for Slide Form
* Fixed bug in campaign stats calculation from refactor
* Refactor lead stats to not use tenant loop
* Better coordinated cron runs
* Added clean up job

#August 3, 2017

* Fixed sorting issue with lead table
* Added Maintenance class to handle deleteding expired data
* Fixed bug in Link Tracking

#August 2, 2017

* Added support for live test for popups
* Fixed enabled/deleted bug in popup
* Allow HTML in title and body when editing
* Strip html from title in list display
* Added check to allow html in cleanInput
* Expanded margin settings
* Added more css options to popup json
* Added unit tests for popup and redirects
* Refactored CampaignStats from 25s run time to < 3s
* Added column to ds_Redirect for Tenant
* Added support for compression of CSS and JS in Release mode
* Fix for date time offset in common formatting
* Updated image management to ensure image is saved in same format sent
* Fix bugs in invite/delete users


#August 1, 2017

* Rolled out exit intent 2.0
* Fixed some bugs with exit intent 2.0