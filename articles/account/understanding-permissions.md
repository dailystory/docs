{
title: 'Permissions',
description: 'Understanding Role Permissions in DailyStory'
}
# Understanding Role Permissions in DailyStory
DailyStory supports a robust permissions model used to control what [users](/account/users) can do. Users are assigned to [Roles](/account/roles) and Permissions are granted to users in those roles.

## Default Permissions
If no Roles are enabled, DailyStory defaults to all users being granted Administrative permissions. For many customers, this is the recommended configuration. This ensures that all users have the ability to manage their DailyStory settings and configuration.

> The statement "Roles are enabled" means that a role has been created. If no roles exist, then roles are considered disabled.

If Roles are enabled, the DailyStory uses permissions to control access.

## Permission-based Access
DailyStory's permission system is a grant-based permission model. This means that when roles are enabled users must be granted permissions to perform actions.

### Site Owner Permission
There is a single "Super User" account known as the Site Owner. The Site Owner is configured in [Account Settings](/account/settings). The Site Owner is always granted Administrator-level permissions and cannot be deleted from the list of [users](/account/users) for the application.

> The Site Owner is a fail-safe account to ensure you cannot be locked out of your DailyStory account.

The Site Owner permission is set by selecting a user in [Account Settings](/account/settings).

### Administrator Permission
While the Site Owner is always granted Administrator-level permission, a Role can also be granted Administrator permission thereby giving users in the role Administrator permissions.

To create an Administrator role, create a new [Role](/account/roles), and check `Administrator`:

![Administrator Permissions](/articles/account/permissions-01.png "Administrator Permissions")

By checking `Administrator` this will also automatically check all other permissions to indicate that these permissions are also being granted.

> While checking all other permissions other than `Administrator` grants similar rights, this doesn't give access to administrator features.

#### Administrator-only Features
The `Administrator` permission also grants access to the Admin section of your DailyStory application. Features such as configuring roles, adding users, enabling integrations, setting site options, creating API keys and more are all restricted to the `Administrator` permission.

### Application Permissions
Application permissions grant users in the role the ability to either view or manage features. 

These permissions are identified as:

* `[Feature Name]CanView` - view items related to the feature
* `[Feature Name]CanManage` - view, create, or edit related to the feature

> The `[Feature Name]CanManage` includes the `[Feature Name]CanView` permission. Granting both is unncessary.

Feature-level permissions include:

* Campagin
* Contact
* Content
* Segment

#### Example Application Permission
A user in a role that has been granted the `CampaignCanView` permission, but not the `CampaignCanManage` permission has the ability to view campaigns. However, if an attempt is made to edit the campaign, add a lead, edit a workflow, or anything else related to changing the campaign a Access Denied error message is shown:
	
![Access Denied](/articles/account/permissions-02.png "Access Denied")

## Common Role Configurations
If you choose to enable roles we recommend creating two roles:
	
* Administrators - grant this role the `Administrator` permission and add yourself and other users that need this permission to it.
* Users - grant this role the default set of permissions all users should have. Add all users to this role.
	
## Frequently Asked Questions
Below are some frequently asked questions.

### A user is in two roles, which role grants their permissions?
DailyStory is designed to grant the highest level of permission given by the roles a user belongs to. If a user in in multiple roles and the first role does not grant a permission, e.g. `CampaignCanManage`, but the second role does grant it, the user is given `CampaignCanManage` permission.

### Does the name of the role matter for permissions?
No, but we recommend using names such as "Administrator" or "Content Editors" to help indicate what the role is used for.

### Can I have two roles with the same name?
No, you are not allowed to have two roles with the same name.

### A role's permission was changed, when will it apply to the users?
Permissions are granted per-session. Therefore changes in a role's permissions are applied the next time the user logs in.

### I changed permissions and locked myself out of the site
Contact your site owner, they will need to login and add your account to an appropriate role to grant you the permissions you need.
