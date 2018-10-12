{
title: 'Roles',
description: 'Roles control what users can do in DailyStory'
}
# Roles in DailyStory
A role is used to identify a group of [Users](/account/users) that share a common set of permissions within a DailyStory account.

> If roles are not used, all users are considered Administrators and have full access to all features of DailyStory.

Roles are managed in the Manage Roles screen in the administration section of your account.

![Manage Roles](/articles/account/roles-01.png "Manage Roles")

> Important, if you decide to enable roles ensure your account is granted Administrator permissions or you are the Site Owner.

## Add a Role
To add a new role click the + Add Role button. This opens a popup where you provide the name of the role to add:
	
![Add Role](/articles/account/roles-02.png "Add Role")

Clicking the next button creates the role and opens the Manage Role screen:
	
![Manage Role](/articles/account/roles-03.png "Manage Role")

## Manage a Role
The Manage a Role screen is used to add users to the role and define the permission for the role.

### Add a User to a Role
To add a user to a role, click the + Add User button in the Manage Role screen. This opens a popup that shows a list of users not currently in the role:
	
![Add user to role](/articles/account/roles-04.png "Add user to role")

Select the user or users to add to the role and cick the Add button. The Manage Role screen will update the list of users in the role:
	
![Manage Role](/articles/account/roles-05.png "Manage Role")

### Remove a User from a Role
To remove a user from a role, click the Remove button next to the user to remove in the Manage Role screen. 

> You will need to click the Remove button twice to confirm.

### Grant Permissions in the Role
The main purpose of roles is to grant groups of users permissions to features within DailyStory. Roles can also be used to restrict features from users.

For more information about permissions, please see [Understanding Permissions](/account/understanding-permissions) in DailyStory.

To grant permissions, check the permission you want users in this role to have. To restrict permissions, uncheck the permissions the user should not have.

For example, to grant users of a role the permission to create and edit [Campaigns](/campaigns), grant the `CampaignCanManage` permission. 

Conversely, if you don't want certain users to have the ability to edit Campaigns add them to the role, but do not check `CampaignCanManage`.

## Delete a Role
To delete a role, click the Delete button in the Manage Role screen.