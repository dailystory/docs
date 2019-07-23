{
	title: 'June 2019 Product Update',
	description: 'Product Updates for June 2019'
}
# DailyStory Product Updates for June 2019
## June 28, 2019
* Bug: missing method attribute
* Refactor: handle interactions after upload
* Refactor: style updates for file manager
* Bug: handle folder deletes
* Refactor: set focus on file manager create folder
* Refactor: style changes and elipses on file manager
* Refactor: content copy edit

## June 27, 2019
* Bug: multiple refreshes of large select box causing perf issues
* Bug: additional bug fixes to scheduler
* Refactor: update styles for ellipse buttons; table header updates
* Refactor: update archive icon and ellipses
* Refactor: hide extra column on responsive

## June 26, 2019
* Bug: handle issue where import please wait didn't turn off
* Bug: escape symbols in environment files
* Refactor: add support for geo searches less than 1 mile
* Refactor: add support for batch lookup queries for contacts
* Refactor: update testability of bulk import

## June 24, 2019
* Refactor: convert to use GetAssetsAsync
* Refactor: remove create folder from picker
* Refactor: updates for unit tests; change models
* Refactor: track unsaved changes in page editor
* Refactor: change button behavior for emails; and default to design
* Bug: unsaved changes not reset after save
* Bug: fix issue with duplicate css classes

## June 19, 2019
* Refactor: continued UX updates
* Refactor: remove tracking tag from main drop down
* Bug: matches could be null
* Refactor: add delete for file asset
* Bug: import could create non-public container
* Refactor: remove contentpagedesigner
* Refactor: update image store with save preview
* Refactor: don't force images to 100% width in file picker
* Refactor: add reset option to designer; address style bugs; refactor storage manager
* Bug: secondary button style

## June 18, 2019
* Refactor: add file picker in to email editor
* Bug: span is a valid text type in page designer
* Bug: import with file wasn't persisting segment id
* Refactor: change content page controller to use streams
* Bug: not handling null designer object properly
* Refactor: css updates and move add assets to modal
* Bug: didn't close bracket on import
* Refactor: add assset modal for selecting assets in campaign
* Refactor: data table view should allow search text to be set
* Refactor: convert views to new sidebar menu layout
* Refactor: move campaign side bar to partial
* Bug: stop limiting dynamic segments to only active members
* Bug: pages didn't load associated css urls into designer
* Refactor: change page index to fluid

## June 15, 2019
* Upgrade to latest version of grapesjs
* Refactor: updates to email designer
* Refactor: more turns on email designer
* Refactor: updates to footer component for email

## June 14, 2019
* Refactor: convert to native grapejs component storage
* Refactor: fold components into separate file; bug in div formatting

## June 13, 2019
* Refactor: add viewport meta tag

## June 12, 2019
* Bug: fix bug in Mindbody Sync table
* Refactor: don't log exceptions in debug
* Bug: fix invalid html in content updates for designer
* Refactor: content page box to block
* Refactor: more styke clean up

## June 11, 2019
* Refactor: add support for screen shots to designer
* Refactor: add reports column
* Refactor: add support for preview button
* Refactor: mouse enter/exit for edit html
* Refactor: text clean up and polish
* Refactor: preview on html editor
* Refactor: remove dead files
* Refactor: handle loading related css files for preview and published
* Refactor: changd from Dimension to styles
* Refactor: style updates and add splash
* Refactor: fix bugs in designer
* Refactor: integrate file picker with page designer
* Refactor: updates for designer picker
* Bug: include preview flag in preview urls
* Bug: content page settings should be empty string
* Bug: slug should be set if empty
* Refactor: ContentPage methods
* Refactor: users
* Refactor: update cms to allow cache invalidation of pages
* Refactor: update WordPress plug-in to support site url setting

## June 10, 2019
* Refactor: continue updates in content page refactor branch
* Refactor: cancel behavior and css updates
* Refactor: add container support
* Remove: old references in acquisition controller
* Bug: bad paths for popups
* Refactor: add support for editing image
* Bug: campaign id not getting set; edit vs create mode
* Bug: handle design/html clicks vs links; page id from save
* Bug: wrong location for table clicks
* Bug: head may be null on create
* Refactor: page gallery part of save settings
* Bug: column singular
* Refactor: support draft pages with disabled submit
* Refactor: add UX for web form and published status

## June 7, 2019
* Bug: handling casing on url hashing
* Bug: handle inner html updates to grapesjs component
* Refactor: keep attributes on selection
* Bug: empty models when a component is updated

## June 6, 2019
* Bug: fix check for empty collection
* Refactor: updates for unit testing
* Bug: refactor and missing check on image width
* Bug: use date first sent for export report
* Bug: stats report is already cached
* Refactor: update webjobs webhooks
* Bug: support legacy email hash

## June 5, 2019
* Refactor: webforms updates for unit tests
* Refactor: webhooks updates for unit tests
* Refactor: roles updates for unit tests
* Bug: handle empty string condition in templating
* Refactor: clean up controllers and remove unused

## June 2, 2019
* Add: support for @ helper in handlebars