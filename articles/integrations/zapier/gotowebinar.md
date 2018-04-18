{
	title: 'DailyStory + GoToWebinar integration',
	description: 'Setting up GoToWebinar integration with DailyStory using Zapier'
}
# DailyStory + GoToWebinar integration using Zapier
Using DailyStory's [Zapier integration](/integrations/zapier/) you can connect many differnt types of applications together.

The DailyStory + [GoToWebinar](https://www.gotomeeting.com/webinar) integration shares registrant and attendee data with your DailyStory campaign. It eliminates the need to export/import CSV lead data from your GoToWebinar meetings.

Below are instructions for configuring common DailyStory + GoToWebinar use cases using Zapier.

## Capture GoToWebinar Attendees
Below are the steps for capturing GoToWebinar attendee data in DailyStory.

<ol class="step"><li value="1">Create a GoToWebinar Trigger</li></ol>
Create a new Zap and add the GoToWebinar Trigger: New Attendee. Configure the trigger with the correct webinar:

![DailyStory + GoToWebinar Create Trigger](/articles/integrations/zapier/gtw-zapier-01.png "DailyStory + GoToWebinar Create Trigger")

<ol class="step"><li value="2">Create a DailyStory Action</li></ol>
Add the DailyStory Create or Update Lead Action to your Zap:
	
![DailyStory + GoToWebinar Create or Update Lead Action](/articles/integrations/zapier/gtw-zapier-02.png "DailyStory + GoToWebinar Create or Update Lead Action")

Configure the DailyStory Create or Update Lead Action to create or update leads in your DailyStory campaign. Then select the email address received from the GoToWebinar Trigger and any other information, such as the person's name.

![DailyStory + GoToWebinar Create or Update Lead Action](/articles/integrations/zapier/gtw-zapier-03.png "DailyStory + GoToWebinar Create or Update Lead Action")

<ol class="step"><li value="3">Create a DailyStory Action</li></ol>
Add another DailyStory Action, Add Lead Activity, to your Zap. Configure the Action to use the Lead Id received from the Create or Update Lead Action created in Step 2:
	
![DailyStory + GoToWebinar Add Lead Activity](/articles/integrations/zapier/gtw-zapier-04.png "DailyStory + GoToWebinar Add Lead Activity")

<ol class="step"><li value="4">Save your Zap</li></ol>
Save your Zap. When people attend your webinar new leads will be created in DailyStory or existing leads will be updated. Next, the lead will include an activity identifying that they attended your webinar.