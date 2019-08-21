{
	title: 'DailyStory + Verint Community',
	description: 'Integration for DailyStory and Verint Community'
}
# DailyStory + Verint Community
The DailyStory + Twilio integration enables you to use the power of DailyStory's marketing and automation tools with a powerful online community platform: [Verint Community](https://www.telligent.com/).

When enabled, this integration allows you to: 

* Create audience segments from Verint Community members.
* Identify prospective customers in your Verint Community.
* Run more effective welcome campaigns to Verint Community members
* Re-engage inactive members in your Verint Community

And more! You can [read more about all these capabilities here](https://www.dailystory.com/telligent-community-integration/).
	
## Configuring Verint Community Integration
There are several steps required to configure DailyStory and Verint Community integration. These steps are detailed below.

<ol class="step"><li value="1">Install plug-in</li></ol>
[Contact DailyStory](https://www.dailystory.com/contact-us/) and request the Verint Community plug-in. This plug-in ensures that activities by community members can be properly associated with a user in DailyStory.

Once the plug-in is installed, you will need to provide a DailyStory API key and the cookie domain

![Verint Community plug-in](https://www.dailystory.com/wp-content/uploads/2018/10/Telligent_1.png "Verint Community plug-in")

Once the plug-in is installed in Verint Community, set the API key (from DailyStory) and optionally set the cookie domain. The DailyStory API key is generated and managed in the admin panel of DailyStory.

<ol class="step"><li value="2">Configure integration</li></ol>
Next, sign in to your DailyStory account and navigate to integrations. Select Telligent and enter the API end point https://[your domain]/api.ashx/v2/ and a Verint Community API Auth key and user:

![Verint Community integration in DailyStory](https://www.dailystory.com/wp-content/uploads/2018/10/Telligent_2.png "Verint Community integration in DailyStory")

Once this is complete, DailyStory will synchronize with the contacts in Verint Community once every 3-hours.

Note: Verint Community integration is only available for DailyStory customer's on a Premium or greater licensing plan.

## Frequently Asked Questions
Below are some frequently asked questions.

### How often will data sync from Verint Community to DailyStory?
Sync runs once every 3-hours. When initially setup, please contact us an request an initial sync - we'll go back and sync up to 18 months of records.

### If a community member is opted out of emails, does DailyStory honor that?
Yes, users that have opted out of emails in Verint Community are automatically opted out of emails in DailyStory.

### What fields does DailyStory capture from the community?
Below is the list of fields currently imported from Verint Community into DailyStory. Fields such as roles, groups and achievements, points, total posts, last visit date and join date are all available for building filtered segments in DailyStory.

* Name
* Company
* Title
* Date of Birth
* Address
* City, State/Region, Country, and Zip/Postal code
* Gender
* Home Phone
* Mobile Phone
* Account Status (Anything other than "Active", will flag the contact in DailyStory as "Inactive")
* Avatar / User Photo
* User Roles
* User Groups
* User Achievements
* Total Point count
* Total Post count
* Telligent Id
* Join date
* Last visit date
