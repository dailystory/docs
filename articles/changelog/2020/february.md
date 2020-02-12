{
	title: 'February 2020 Product Update',
	description: 'Product Updates for February 2020'
}
# DailyStory Product Updates for January 2020
## February 12, 2020
* update wait until time passed workflow logic
* bug in next process wait until logic

## February 10, 2020
* Refactor: adjustments to licensing to support onetool
* Refactor: add support for onetool api
* Refactor: remove preview tag from autopilot
* Refactor: add support for contact tags
* Refactor: fix bugs in workflow to ensure emails are sent out and popups are triggered
* Add completed and waiting counts to automation list
* responsive design columns for autopilot

## February 9, 2020
* Refactor: reorg web project with autopilot reference
* Refactor: bug in delete workflow path; auto set name and description if not set
* Refactor: some triggers cannot start automation
* Refactor: add support for total complete / waiting

## February 8, 2020
* Refactor: re-org as autopilot for workflow vnext
* Refactor: time triggers not async

## February 7, 2020
* Refactor: neverbounce had bad url path
* Refactor: add in support for popup completed and popup api controller
* Refactor: update url on save for new workflows
* Refactor: clean up workflow
* Refactor: bug in waittime key value
* Refactor: scope popups to campaigns
* Refactor: start work on skip/take for processing workflow
* Bug: condition wasn't handled for yes/no
* Refactor: return list instead of dictionary for workflow step lookup
* Refactor: bug in how datetime was handled in sms replies view
* Refactor: don't auto reply to sms if there is a rule
* Refactor: missing condition for hastextmessagereply
* Refactor: trigger to look through list not dictionary
* Refactor: add support for condition to evaluate text message reply
* Refactor: fix various ux bugs with workflow

## Feburary 6, 2020
* Refactor: warm up segments and campaigns for contact detail

## February 5, 2020
* Refactor: add support for friendly name to all blocks
* Refactor: add support for assign points to workflow
* Refactor: updates for assign points
* Refactor: remove CampaignRule
* Refactor: remove RunAutomations from project
* Refactor: remove dead code from workflow updates
* Refactor: clean up rules
* Refactor: custom rule set any/all match type
* Refactor: remove event listeners after use
* Refactor: fix bug in max value for date; updates for geo
* Refactor: add method to find campaign by name
* Refactor: add routing to a workflow
* Refactor: add when popup is completed
* Refactor: add trigger to lead creation
* Refactor: fix old bug in old workflow

## February 4, 2020
* Refactor: handle case when no lead for dsid
* Refactor: set ruleset on save
* Refactor: change returned exception type when invalid
* Refactor: add support for add/remove points action
* Refactor: remove score and automation replace with new workflow

## February 3, 2020
* Refactor: mouse pointer interaction on block elem hover
* Refactor: add when text message replied and has reply text
* Refactor: add yes no condition
* Refactor: add support for text message replied trigger
* Refactor: fix bug in date time picker
* Refactor: methods for calculating distance between 2 geo points and finding closest
* Refactor: add support for closest sub account by geo
* Refactor: add support for lead routing
* Refactor: handle scroll offset when block list div is scrolled
* Refactor: do unsaved changes in workflow
* Refactor: normalize names
* Refactor: add support for custom rules
* Refactor: clean up how custom rules are supported
* Refactor: load in custom rules
* Refactor: undo rule selector changes to v1
* Refactor: new RuleSet
* Refactor: handle merge conflict in process rules
* Refactor: add support for hascustomrule
* Merge workflow vnext into staging
* Refactor: support campaign filtering
* Refactor: add view for all workflows

## February 1, 20202
* Refactor: fix offset position with workflow indicator
