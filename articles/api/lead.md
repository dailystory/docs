{
	title: 'DailyStory Lead REST API',
	description: 'Documentation for DailyStory\'s  Lead REST API'
}
# Lead REST API
Use the Lead REST API to create or find leads in DailyStory campaigns.

> Impor

## Create a Lead
To create a lead you need to have an email address and the `Id` of the campaign the lead is either in or will be created in.

Step 1 - create an API key: 
https://us-1.dailystory.com/Admin/ApiKeys

Step 2 - create an HTTP basic header
The value of the header should be a Base 64 encoding string "api:[your api key]".

Step 3 - send a GET request to get a lead
For example, to get this lead:
https://us-1.dailystory.com/API/Lead/117427

Step 4 - send a POST request to create a lead
https://us-1.dailystory.com/API/Lead/
The body can be the full representation of the lead or as simple as -- we require the campaignid and an email address. You can find the campaign id by viewing a campaign in your browser and you'll see the id in the URL:

{
            "campaignId": 69,
            "email": "9d9dsftest@example.com",
}