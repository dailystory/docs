---
layout: _ArticleLayout
title: May 2017 Product Update
description: Product Updates for May 2017
---
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
