{
	title: 'DailyStory About REST API',
	description: 'Documentation for DailyStory\'s  About REST API'
}
# About REST API
Use the About REST API to get information about the DailyStory API.

## GET /api/v1/about
Used to return information about the DailyStory API.

### Sample response body
Returns a JSON API response with the current date time, name of the tenant, Unique ID of the tenant and the Data Center the tenant is running in.
	
<pre class="brush: javascript">
{
	"Status":true,
	"Message":"",
	"Code":200,
	"Response":
	{
		"timestamp":"2019-10-27T19:14:45+00:00",
		"tenant":"Unit Test Account",
		"uid":"ghg0ctulvdx7bu10",
		"dataCenter":"us-1"
	}
}
</pre>