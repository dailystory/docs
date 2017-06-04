---
layout: _ArticleLayout
title: June 2017 Product Update
description: Product Updates for June 2017
---

# June 3, 2017

* Remove campaign functionaliy was marking lead as rejected, when should have been deleted
* Update lead stats job to flag bounced contacts
* Add Bounced status for Contact status
* Add Account class initial check-in
* Add AccountId and Account APIs on Contact objet
* Update import logic to flag imports as 'imported' and ignore exceptions
* Reformat email activity item SQL
* Add AccountId to lead
* Add account not found exxcption to lightning exceptions
* Add /Account controller and AccountModel
* Removed existing account functionality to move to admin controller
* Add Index and Detail for Account controller
* Updated Remove Lead logic to delete not mark as rejected

# June 1, 2017

* Updated logic in web forms javascript to detect if Recaptcha script is already loaded.
* Added a 404 check in localhost mode for debugging
* Fixed a bug in web form slug check that was looking for null and not empty string
* Added async event handler on request demo button to dailystory.com to verify functionality