{
	title: 'November 2018 Product Update',
	description: 'Product Updates for November 2018'
}
# DailyStory Product Updates for November 2018
## November 6, 2018
* Refactor: clean up OwnerId in Account
* Feature: updates to Account
* Refactor: fix build warning
* Refactor: fix GetTenant for user
* Refactor: Performance improvements for bulk import
* Bug: handle whitelabel redirect on password reset

## November 6, 2018
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
