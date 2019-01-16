{
title: 'Personal Settings',
description: 'Configure your Personal Settings in DailyStory'
}
# Personal Settings
Personal Settings enable you to configure options related to your login account for DailyStory. This includes setting such as email address, timezone, notifications and more.

![Personal Settings](/articles/account/personal-settings-01.png "Personal Settings")

## Contact
The contact section of your Personal Settings are used by DailyStory to configure where emails and text messages may be sent to. If services such as Text Message are enabled for your account, the mobile number you specify is used to send confirmation text messages and is the default for any test Text Messages you wish to send to yourself.

> Important - Email is required to create a user in your account.

When using features such as Text Messages that requires [Twilio integration](/integrations/twilio), your mobile number must be set to complete the configuration.

## Timezone
The timezone determines how dates and times are shown and is also required when creating scheduled activities (emails, text messages, and so on). If your timezone is not set, DailyStory will default to the timezone found in your [Account Settings](/account/settings). If timezone is not set in Account Settings or Personal Settings, DailyStory will default to UTC time.

## Display Options
Use Display Options to configure how DailyStory will display values such as money, dates and times.

> Important - DailyStory does not manage currency conversions.

## Notifications
There are many types of notifications that DailyStory sends. Two of these notifications are New Lead Notifications and Daily Summaries. 

The New Lead Notification is sent whenever a new inbound lead is created in any campaign. For example, if a [Magic Form](/acquisition/magic-forms/) is configured for a contact form on your website, whenver someone completes the form and DailyStory receives the lead you will be sent a New Lead Notification. By default, new users in DailyStory are subscribed to New Lead Notifications.

The Daily Summary email is a digest email of all activities that occurred the previous day. It is sent at 7:00AM every morning and contains  metrics such as: leads created, page visitors, website sessions and more. It also includes a list of the leads (up to 25), a list of returning contacts (up to 25) and, when enabled, a list of identified anonymous visiting companies. By default, new users in DailyStory are not subscribed to Daily Summary emails.

To opt out of Daily Summary New Lead Notification emails, turn the respective notifications to off:

![Notifications](/articles/account/personal-settings-02.png "Notifications")	
	
## Sign in Account
If you manage multiple accounts within DailyStory you can identify which account is the account you are logged into when you sign in to DailyStory.

## Frequently Asked Questions

### How do I disable notifications for someone on my team?
Not everyone on your team may want or need notifications when new leads are created. To disable notifications these users can log in to DailyStory and [disable their Notifications](/account/personal-settings#notifications). If you are a site owner you can also disable notifications for them. In Account Settings navigate to Users. Click on the user whose settings you wish to modify. Change their notification preferences and click Save.

### Can I opt in to lead notifications for specific campaigns?
Unfortunately not at this time. We are considering this as a future option.

### How do I change a password for someone on my team?
You cannot change the password for someone on your team. However, you can send them a link to reset their password. In Account Settings navigate to Users. Click the Re-Invite button next to a user. This will send a link to the user which they can use to reset their password. Alternatively, anyone can go to the [Forgot Password page](https://app.dailystory.com/forgotpassword) and request for their password to be reset.

### What happens if someone resets my password for me?
If someone, other than yourself, attempts to reset your password you will receive a Reset Password Notification to the email configured with your user account in DailyStory. However, until your password is changed, your existing password will continue to work. If you receive unwanted or unexpected emails to reset your password, someone may be attempting to gain access to your account. If this happens, [please let us know](https://www.dailystory.com/contact-us/).

### Why are the dates and times shown different than my local date and time?
If the dates and times shown next to any record in DailyStory does not appear to be correct, this may be because either your account timezone or your personal timezone have not been set correctly. All dates and times in DailyStory are stored in UTC, they are converted to your local date and time (timezone) by settings first in your [Account Settings](/account/settings) and then in your [Personal Settings](/account/personal-settings#timezone).

### How do I change the format used for dates and times?
To change the format used for dates and times, simple choose from the list in the Display Options of your [Personal Settings](/account/personal-settings#display-options).