{
	title: 'November 2019 Product Update',
	description: 'Product Updates for November 2019'
}
# DailyStory Product Updates for November 2019
## November 12, 2019
* Refactor: MINDBODY online icon
* Bug: send emails needed negative minutes back
* Refactor: heatmaps on separate bullet in reports
* Refactor: support recently sent emails
* Refactor: adjust back button font in login.css
* Refactor: set default calendar view to week
* Refactor: main event calendar filtered to today
* Refactor: color highlight calendar
* Bug: fix issues to support mce 5
* Refactor: switch mindbody icon

## November 11, 2019
* Bug: slug could get set to empty string
* Bug: LeadQueue must specify data center
* Refactor: set RedirectUrl to empty if message is action type
* Refactor: stub function for generating secret proof in Facebook
* Refactor: convert from sproc
* Bug: web forms should only return active
* Refactor: add email instrumentation
* Refactor: update MBO sync hourly
* Refactor: email instrumentation to handle better granularity
* Refactor: update graphs automatically
* Refactor: update instrumentation routes
* Refactor: side bar menu as partial
* Refactor: more updates to email instrumentation
* Refactor: use utc for moment.js
* Refactor: json dates handling for reports
* Bug: timezones in email instrumentation

## November 10, 2019
* Refactor: updates to instrumentation

## November 8, 2019
* Refactor: enable webform with embedded message
* Bug: allow access control origin

## November 7, 2019
* Refactor: schedule.js to bubble error messages
* Bug: check if campaign is valid before scheduling
* Refactor: opt out of parent if contact in child unsubscribes
* Refactor: GetStatsAsync for campaign
* Refactor: email instrumentation
* Bug: handle nulls for campaign stats
* Refactor: warn when there are no leads in the campaign

## November 6, 2019
* Refactor: async campaign lookup
* Bug: handle case where title and body html are empty
* Bug: set slug if not specified
* Bug: exported popup is active
* Refactor: add GetStatsAsync to campaign for API
* Refactor: api namespace
* Refactor: campaign api
* Refactor: convert auto archive to sproc
* Refactor: update libs for cms
* Refactor: update mailgun spools

## November 5, 2019
* Refactor: don't set button target for pages
* Bug: updates to preheader

## November 4, 2019
* Refactor: display errors when creating trial
* Refactor: better handle error messages
* Bug: ignore emails with a test dsid for status