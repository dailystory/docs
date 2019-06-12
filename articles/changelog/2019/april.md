{
	title: 'April 2019 Product Update',
	description: 'Product Updates for April 2019'
}
# DailyStory Product Updates for April 2019
## April 29, 2019
* Bug: allow mailto links to pass through for email url rewrite
* Refactor: add support for telligent groups and achievements
* Refactor: more unit tests for Mindbody sync
* Refactor: more unit tests and coverage for Telligent sync

## April 25, 2019
* Refactor: add license check for redirects; add policy headers
* Refactor: updates to reorganize Mindbody sync for unit tests

## April 24, 2019
* Refactor: update installer for new Telligent fields
* Bug: send delay wasn't in the right place
* Bug: activity checked for not null when should check for null
* Refactor: add new properties for telligent sync
* Refactor: update jobs manager to handle default days back

## April 23, 2019
* Bug: contact country and timezone not properly set
* Refactor: show company name in title if present
* Bug: graph fields for string array and double not handled
* Refactor: Telligent - fix reference bugs and update for more profile field types

## April 22, 2019
* Bug: issue when link was relative
* Refactor: updates for sms link tracking
* Bug: link id should handle case when no lead is found

## April 19, 2019
* Add: base 36 encode / decode
* Add: click tracking for text message queues

## April 18, 2019
* Refactor: update coupons to be cos specific

## April 17, 2019
* Refactor: add support for decimal
* Refactor: integrate NeverBounce into trial
* Bug: use TLS 1.2
* Refactor: add support for DS account
* Refactor: update web stats
* Refactor: update remove user
* Refactor: add auto archive campaigns
* Refactor: better responsive layout for campaigns
* Bug: dates not formatting to local string
* Bug: javascript date format using moment
* Bug: start and end dates
* Bug: no hamburger menu on conversion report
* Bug: stripe update for invoices
* Refactor: support user entering email for upgrade
* Refactor: click support from campaign to email report
* Bug: handle upgrades to license without degrading custom license COS
* Refactor: support account name in new account
* Bug: handle date filtering by date not by datetime

## April 15, 2019
* Bug: fix issues with dates in bar charts
* Bug: add send delay for twilio
* Refactor: log reason for failure
* Refactor: add twilio status code
* Bug: sms detail report link
* Bug: handle exceptions for emails that don't have report data
* Bug: message wasn't setting url correctly
* Added: failed and optout reports for sms
* Refactor: added exports and new controllers
* Bug: IsSmsEnabled and IsPushEnabled should default to true
* Refactor: throw exception is report isn't valid
* Refactor: add methods for new reports
* Refactor: add total_clicked field
* Refactor: start updates to conversion funnels
* Refactor: Lead Summary report
* Refactor: reports controller

## April 14, 2019
* Refactor: store, subscription, coupon updates for Stripe
* Refactor: better error messages for rule
* Bug: validation should handle exceptions
* Bug: merge extended properties
* Bug: reports should show item detail
* Refactor: set coupon in querystring and allow upgrades

## April 11, 2019
* Bug: use ip instead of dsid for outbound link reporting
* Bug: count ips not dsids
* Refactor: report icon no text and date without time
* Refactor: better report detail for page
* Refactor: better report detail for links
* Refactor: NeverBounce integration
* Bug: datamanager skipped cache lookup
* Performance: performance improvements to email sending

## April 10, 2019
* Refactor: reports to use common base controller class
* Refactor: periscope report
* Refactor: handle exceptions
* Add: SmsDetailReport
* Refactor: convert Periscope report

## April 9, 2019
* Refactor: get system event and exception logs
* Refactor: popup reports and add summary report
* Refactor: click fraud report
* Refactor: update link tracking reports and verifying data
* Refactor: web page reporting verification
* Refactor: update link tracking reports
* Refactor: update popup reports
* Refactor: update web reports
* Refactor: update reports controller
* Refactor: update links and paths for reports
* Refactor: sms reports
* Bug: conversions multiplied time 100
* Refactor: add total_optouts for sms
* Refactor: add fitlering for text messages and optouts

## April 8, 2019
* Refactor: move web reports to dedicated controller and consolidate
* Refactor: update references to web reports urls
* Refactor: normalize breadcrumb styles in reports
* Bug: fix search display to be responsive
* Refator: move some functions from reportbase to common
* Refactor: rename and update web reports logic
* Refactor: convert PageInfo report to PageView report
* Refactor: Days in report base calculation

## April 5, 2019
* Refactor: normalize panel box callouts in reports
* Bug: localize dates in email reports
* Add: report for bounce reason
* Bug: Fix broken links to old Email Summary reference
* Refactor: updates reporting javascript to add colors to panels
* Add: delivery summary report
* Refactor: unit testing
* Bug: broke email cloning with perf improvements
* Refactor: add summary detail reporting kpis

## April 3, 2019
* Bug: email click activity only returned the first record
* Bug: report base should set start ends to min val
* Refactor: Data table reports uses custom pager
* Bug: email report should start with date email first sent
* Add: report for which links were clicked
* Bug: email summary report should use bar chart
* Refactor: email delivery details
* Add: NeverBounce integration support
* Refactor: convert link summary report to new report ux
* Refactor: testing for EmailClick items
* Refactor: cache email open report
* Refactor: move email summary; optimize email performance
* Bug: remove status from summary report
* Refactor: email reporting

## April 2, 2019
* Refactor: updates to text messages for notification subscribers
* Refactor: email reports controller for testability
* Refactor: update datatable javascript to handle custom info
* Refactor: convert to use start/end for date filtering
* Refactor: datatable report support breadcrumbs
* Bug: clone should include description
* Bug: do not allow export of empty email report
* Bug: send friendly response to verify twilio webhook is configured

## April 1, 2019
* Bug: web application should throw and handle authentication exception
* Refactor: don't delete dead queue items
* Bug: list to csv stream shouldn't throw an exception