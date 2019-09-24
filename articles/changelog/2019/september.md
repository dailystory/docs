{
	title: 'September 2019 Product Update',
	description: 'Product Updates for September 2019'
}
# DailyStory Product Updates for September 2019
## September 24, 2019
* Refactor: lazy load templates

## September 22, 2019
* Refactor: extract attribute value from css style

## September 21, 2019
* Refactor: remove unused libs
* Bug: fix bugin set parent link for images
* Refactor: designer toolbar button background
* Bug: handle new image components that have src and title
* Refactor: convert header component to use header tag
* Bug: set webformid to 0 if undefined or null
* Bug: fix avoidInlineStyle bug with grapesjs
* Refactor: add PreMailer to main library
* Refactor: bubble up remove to clean up html
* Bug: set image src in image preview
* Refactor: enable mce color pickers
* Refactor: remove built in menus for tinymce 5
* Refactor: add apis for email templates and templates in email index
* Refactor: style for template gallery
* Refactor: set default background color

## September 19, 2019
* Refactor: ensure head tags are set for designer emails
* Refactor: move email html processing into new class
* Refactor: don't allow dropping on button
* Bug: email preview doesn't require manage permission
* Bug: page designer preview button was broken
* Bug: bug with setting links on images broke email and pages
* Refactor: remove tinymce code editor for pages

## September 18, 2019
* Bug: bugs in email editor
* Bug: don't allow selection of non-text elements
* Bug: don't get raw html
* Bug: don't get raw html; don't scroll on screenshot
* Refactor: add import/export support to pages
* Bug: twilio integration remove spelling error
* Refactor: added custom delete with close account to Twilio
* Refactor: import/export content; add tenant details after import
* Refactor: update project libs
* Refactor: add import/export email templates
* Bug: divider email components shouldn't be droppable

## September 17, 2019
* Refactor: designer common functions and settings; modal for html editing
* Refactor: updates to move common functions for email and pages
* Refactor: better image editing and edit html
* Refactor: better image editing and edit html
* Refactor: updates to image preview
* Bug: bug in extended properties array check for null
* Refactor: extended property methods for handling date & datetimes
* Refactor: hide buttons when in edit mode
* Refactor: add clear button to clear designer container
* Refactor: better form editing
* Refactor: update block names and ordering
* Bug: fix items not getting unselected
* Bug: campaign segment could get removed when init campaign editor
* Refactor: fix button behavior in head
* Refactor: better handling dates and next recruit logic

## September 16, 2019
* Bug: double brackets in eligibility check
* Bug: could not remove email from trash
* Bug: allow any image to have a URL
* Refactor: content updates
* Refactor: support select none on page and email designer
* Refactor: direct link editor in email

## September 14, 2019
* Refactor: flag to indicate email is an import on model
* Bug: show preview image if we have one for imported emails
* Refactor: add import method on email controller
* Bug: bad errors check on page designer
* Refactor: update menus on page designer
* Refactor: update email view to handle imports
* Refactor: centralize designer styles
* Refactor: enable file manager
* Refactor: handle import in email index view
* Refactor: update designer html to lock if we have components
* Refactor: add support for actual eligibility in d37
* Refactor: additional methods to handle import export
* Bug: better handle contact document string arrays
* Refactor: clean up old app settings
* Refactor: content updates
* Refactor: set title and alt on video
* Refactor: set videos without button
* Bug: html editor needed to set htmlchanged flag

## September 13, 2019
* Refactor: update MBO sync with new job manager
* Bug: Telligent sync could not process tenant correctly
* Refactor: Degree37 sync to use defined min / max dates
* Refactor: update Degree37 sync with new job manager
* Refactor: update job manager
* Reafctor: add support for gzip compression methods
* Refactor: add support for export email
* Bug: fix MBO bug to handle arrays where membership is removed
* Refactor: store actual eligibility date
* Bug: handle empty group code array in Degree37
* Refactor: handle SetExtendedProperties of arrays
* Refactor: import/export for emails
* Bug: line feed in css
* Bug: set alt tags on app store icons
* Refactor: dynamically update alt/title and urls for buttons
* Refactor: add cta button editor

## September 12, 2019
* Bug: fix issues to support multi columns in emails
* Bug: color picker in designer was off screen
* Refactor: add support for email export
* Refactor: sort line height before colors
* Refactor: update menu items and add emai export

## September 11, 2019
* Refactor: bugs in field constants for d37
* Refactor: skip inlining css for emails
* Bug: email vidoe section should be 100% width
* Bugs: handle mce height; handle change state 
* Refactor: editing disabled when components exist
* Bug: normalize font size

## September 10, 2019
* Refactor: add support for color picker to email settings
* Refactor: add lock UX when html editor sees design components
* Refactor: rename BLock to Content Container
* Refactor: allow editing of CSS and ignore HTML edits

## September 9, 2019
* Refactor: add method for handling email address updates in contact
* Bug: wrong reference to email id in copy for designer
* Bug: email common not properly handling redirect for copy
* Bug: editing inline could set contenteditable to false
* Refactor: update menu for email edit html
* Refactor: update menu for email design html
* Refactor: plaintext editor for edit html
* Bug: remove pre-set color for footer design element
* Refactor: inline css with email body
* Refactor: style updates with edit forms css
* Refactor: handle text section composite components

## September 8, 2019
* Refactor: add scheduler to designer and refactor
* Bug: fix title of html editor

## September 7, 2019
* Bug: update preview image; do not remove comments
* Bug: added extra >; plain text updates
* Refactor: add email common
* Refactor: shared modal for send test
* Bug: edit plaintext height width
* Refactor: integrate send test from email common

## Septmeber 6, 2019
* Refactor: preserve &nbsp; in html editor
* Refactor: start re-organizing designer javascript libs
* Refactor: prettify the buttons for undo, redo, etc.

## September 5, 2019
* Bug: don't update designer's style
* Refactor: update bundle for email html editor
* Bug: email js bundle must include html2canvas
* Bug: hold reference while updating video in background
* Bug: email html editor use timer for updates
* Refactor: add support for comments in email designer
* Refactor: updates to save button positions
* Refactor: email menu options
* Refactor: page menu options
* Refactor: copy/save functionality for email edit settings
* Refactor: set initial html and css for new emails
* Refactor: scheduled messages return already sent messages
* Refactor: add support for update from html editor and copy

## September 4, 2019
* Bug: UpdateModifiedIfExistsAsync needed to handle lookups for dsid when the dsid belongs to another tenant
* Refactor: scheduled should list published items
* Refactor: add copy and edithtml actions to email controller
* Refactor: better handling of history and copy behavior
* Refactor: edit html view for emails
* Refactor: updates to email menus
* Refactor: add AfterFloatBox section
* Refactor: redesign email createedit

## September 3, 2019
* Refactor: show error when saving empty email; handle image types with better styles
* Refactor: design overhaul of designer UX
* Bug: handle body content with multiple nodes in emails
* Bug: designer is in preview
* Bug: use styles to set width on email images
* Bug: set default Css for new emails
* Refactor: add initial date can send email

## September 2, 2019
* Refactor: support custom components for video
* Bug: file manager breadcrumb
* Refactor: update email designer container
* Refactor: add support for email component storage
* Bug: file manager preview picker wasn't setting url
* Bug: disable spell check in input forms
* Refactor: move videotype
* Refactor: handle designer components for grapesjs in email class
* Bug: fix design time rendering of videos

## September 1, 2019
* Refactor: add support for videos component