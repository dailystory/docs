{
	title: 'July 2019 Product Update',
	description: 'Product Updates for June 2019'
}
# DailyStory Product Updates for July 2019
## July 20, 2019
* Refactor: remove conversion from campaign and grammar updates
* Refactor: remove text message notifications in campaign and move to texts

## July 19, 2019
* Refactor: how lead notifications subscriptions are managed
* Refactor: remove old toggle notifications
* Refactor: add support for notification options; fix bugs

## July 18, 2019
* Bug: license expiration could be below in min val
* Refactor: update usage report UX
* Bug: update UX layout bugs in admin
* Refactor: file manager style updates and pager

## July 17, 2019
* Refactor: better testability for graph field
* Refactor: add support for array filter item; issues with spaces and splits
* Refactor: campaigns table use custom paging
* Refactor: modal-xl support for file picker; bug with create folder
* Bug: UX issues with email editor from recent style updates
* Bug: file manager not storing content type in blob
* Refactor: move styles to main css library
* Refactor: convert to xl modal and design updates
* Refactor: more details on files; grammar; style updates

## July 16, 2019
* Refactor: tracking links UX to include conversion metrics
* Feature: initial check in for link tracking experiments
* Bug: convert arrays to use filters

## July 15, 2019
* Refactor: continue working through email designer

## July 13, 2019
* Bug: only need to handle string ids for asset types
* Bug: fix screenshots for link tracking
* Bug: handle no campaign activity
* Refactor: minor updates on campaign for testing
* Refactor: new sparkline model for reporting
* Bug: better handling of when image is saved

## July 12, 2019
* Refactor: add file picker to emails and pages
* Refactor: convert email html editor to use file picker
* Refactor: enable file picker in menu
* Refactor: convert page html editor to use file picker
* Bug: fix folder management and dynamic ux
* Refactor: campaigns move to js file and handle pause state

## July 11, 2019
* Refactor: set to run hourly (d37 sync)
* Bug: handle bad dates and deferrals (d37 sync)
* Refactor: add method for cleaning sync table; perf improvements (d37 sync)

## July 10, 2019
* Refactor: add edit html to quick menu on pages
* Bug: handle custom rte and issue with setting html to empty
* Refactor: minor updates to ds script

## July 9, 2019
* Refactor: style updates
* Remove: campaign stats partial
* Refactor: advanced search icon updates
* Bug: ordering of custom css in designer
* Refactor: add support for email csv export
* Bug: page designer html editor referenced old classes
* Bug: specify draggability for text components

## July 8, 2019
* Bug: task notification should allow invited users to be assignee
* Bug: handle link tracking lead with no leadid
* Refactor: remove old chat components
* Refactor: add option to ignore console logging for testing
* Refactor: add support for export option on email summary
* Refactor: design and style updates (branch)
* Bug: use grapesjs save changes
* Refactor: style updates for consistency
* Bug: content update
* Refactor: popup preview
* Bug: change from rem font size

## July 7, 2019
* Refactor: whitelabel sliding cache
* Refactor: more validation range checking
* Refactor: file manager updates
* Refactor: remove roletype enum
* Refactor: file manager model changes
* Refactor: home controller for unit tests
* Refactor: admim controller for unit tests
* Refactor: content gallery items