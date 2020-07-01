{
	title: 'DailyStory API',
	description: 'Getting started with the DailyStory API'
}
# API Authentication token
DailyStory supports a rich and extensive REST API. All of the functionality in the DailyStory platform is accessible through the API. Use of the API requires an authentication token.

## Generate an API Key
To use the DailyStory REST API you will first need an API key. To create an API key login to DailyStory and then go to Account Settings > API keys:

![DailyStory API keys](/articles/api/api-01.png "DailyStory API keys")

From here you can click the "Add Authentication Token" to generate a new token or revoke existing tokens.

> As a best practice, we recommend creating separate tokens for each application integrated with DailyStory.

## HTTP Requests using the authentication token
All requests made to the DailyStory API require 2 pieces of information:

* End point API URL
* Authentication token

### End point API URL
Use of the API requires you to use a specific data center identifier when making an API request. When logged in to DailyStory this can be determined by examining the URL.

For example, https://us-1.dailystory.com uses the 'us-1' data center. Whereas https://uk-3.dailystory.com uses the 'uk-3' data center.

> All API requests are made using the URL that includes your data center, e.g. https://us-1.dailystory.com/api/v1/about

### Authentication token
The DailyStory API requires, and only supports, HTTPS requests using Basic authentication. The authentication token should be set as the `Password` and the `Username` set to "api".

For example:

`curl --user api:384XXXXXXXXXXXXXX-us-1 https://us-1.dailystory.com/api/v1/contact/a761f461f00e4fb98040d0a73733b50d`