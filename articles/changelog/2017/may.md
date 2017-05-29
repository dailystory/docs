---
layout: _ArticleLayout
title: May 2017 Product Update
description: Product Updates for May 2017
---
# May 29, 2017

Bug fixes and improvements to DailyStory JavaScript library 

* Fixed reference problem with mobile and tablet checks.
* Added event for exit (ds_exit)
* Cleaned up some issues with cover in preparation for release

Other fixes / improvements

* Added HTML tab for pages. Much better than tinymce source
* Added tooltips to pages
* Removed code option from pages and email editors
* Added test page for DailyStory javascript API

# May 26, 2017

Number of bug fixes, improvements and stub in a few new features based on customer feedback.

* Updating licensing logic to check for users that do not have a credit card for their account. Example, they paid via invoice.
* Added a new public API for looking up a dsid by email address. This is for one of our Telligent customers for the integration we are building.
* Added a new tracking event to enable customers to create, send and track custom events with their campaigns. Added to the DailyStory JavaScript API.
* Version update for DailyStory javascript API to version 1.3. Added new event tracking logic, new ds_ready event, fixed a bug in sayHello function that cause querystring conflicts
* Big update to web form editing. Simplified and added support for free text within the forms.
* Fixed navigation elements in administration
* Added Text option for web form in enum
* Added GetContactByEmailAsync method that looks up using the site id
* Added EventQueueItem for user events
* Fixed issue in license check, now by passes users in the DailyStory admin role.
* Fixed bug in link tracking to show customer domain if one is mapped to Dailystory
* Fixed bug in PayPerClick Keyword summary that was calculating with MCL instead of MQL
* Fixed bugs in popup reports
* Updated SQL in select users lookup to skip DailyStory admin id


# May 25, 2017

* Added support in Web Forms for adding text in the form
* Added support for horizontal css forms
* Updates to web forms landing page javascript

# May 23, 2017

* Fixed login bug that would appear when switching between logins or if a login existing in another tab.
* Fixed another bug with Debug logic; simple redirect fixed this to ensure cookie and credentials were written out.
* Fixed bug with web form that caused editing the call to action button to change another button's text.
* Fixed bug with web forms that prevented a pre-existing call to action text from getting updated
* Popup reporting had a bug with how it calculated conversions.
* Improvements to popup reporting to use a join to connect with lead table
* Updates to web tracking callback to remove checks for a json string from popup
* Updates to CMS functionality to add support for horizontal web forms
* Fix in Ds Javascript API to handle a case where the popup was not reseting the overflow on the body tag. Still not sure this is 100% addressed.

# May 21, 2017

* Updates to form designer to simplify
* Consolidated form designer css
* Updated licensing flow to match with changes
* Updated email designer for test email to only support a single test message
* Added call to action button in form designer - text box only was bad UX
* Added call to action default value and automatic default if left blank
* Fixed bug in email tester that would cause a double email to be sent in some cases
* Updated text in upload contact to reflect that bulk import can take 10-15 minutes to update
* Improvements to bulk import / lead import jobs to make it much faster. Basically job runs until queue is empty vs. working in sets

# May 9, 2017

Small bug fixes

* Fixed bug in send test email
* Updated contact DsId property to include setter/getter logic for dsid formatting
* Added Api entry as a lead creation type
* Updates to Lead PageView Report
* Some clean-up on aisle 5 (more UX nits with login)

# May 6, 2017
Added support for alternative URL in tracking URLs for Google

# May 3, 2017
A few small updates today that improve overall performance.

* Converted all lead paths to go through queue for faster writes. 
* This also included improvements to the popup.
* Fixed bug in web activity item that was preventing drill down on lead page.
* Added option when creating new lead to not send a new lead notification (e.g. on bulk import)
* A few bug fixes to salesforce integration to handle close date on leads
* Simplified the lead import job

Added new Lead PageView Report

* Provides a list of page views broken down by qualified leads

We also enabled the UK data center.

# May 2, 2017
Updated trial, login and logout pages to simplify them more.

* Changed reset, forgot password, welcome and invitation to use a floating boxy style UX
* Removed the requirement when creating a trial to enter your company name, now just Trial Account"
* Moved common login functionality to login.js

# May 1, 2017
Quite a few updates for the start of May:

A number of improvements and bug fixes to the contact import functionality. Including:

* Support for ignoring the first row in a CSV file in case it contains column headers.
* Support for adding new contacts to a campaign.
* Fixed bug in HTML encoding/decoding when copy/pasting CSV values in text box
* Cleaned up import screen and moved documentation to docs.dailystory.com

Updated Contact export

* There was a bug in contact export that was using the lead format.
* Added additional contact specific fields
* Updated both contact and lead export to move date time stamps to last column

DailyStory JavaScript API

* Minor update to the hello bar, still not ready for public use

Bug fixes and enhancements to popups

* Started wiring in support for layout, but still not enabled in production

Bug fixes and enhancements to utility script

* Added support for loading / unloading state for long running web tasks.

Documentation

* Added link in production navigation to [DailyStory Documentation](https://docs.dailystory.com)
