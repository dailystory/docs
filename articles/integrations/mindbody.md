{
	title: 'DailyStory + MINDBODY ONLINE',
	description: 'Integration for DailyStory and MINDBODY ONLINE'
}
# DailyStory + MINDBODY ONLINE
The DailyStory + MINDBODY ONLINE integration enables you to use the power of DailyStory's marketing and automation tools with the [MINDBODY health and wellness platform](https://www.dailystory.com/mindbody-integration/).

When enabled, MINDBODY integration allows you to sync MINDBODY customer data, fields, memberships, and more directly to DailyStory. Then, use DailyStory’s powerful segmentation and personalization tools to craft targeted messages for your clients.
	
> DailyStory's MINDBODY integration is only available to customers using the Professional or higher version of DailyStory.

## Configuring MINDBODY Integration
There are several steps required to configure DailyStory and MINDBODY integration. These steps are detailed below.

<ol class="step"><li value="1">Obtain MINDBODY Site Id</li></ol>
When you login to your MINDBODY account you can easily find your Site Id in the url. For example:

`https://clients.mindbodyonline.com/home?studioid=-99	`

In the above URL the Site Id is `-99`.

> Your MINDBODY Site Id may be a negative number.

Copy your Site Id and then login to your DailyStory account.

<ol class="step"><li value="2">Configure Site Id</li></ol>
Login to DailyStory and navigate to Admin > Integrations, click on the MINDBODY integration and add your Site Id:

![DailyStory + MINDBODY](/articles/integrations/mindbody-01.png "DailyStory + MINDBODY")

Next, click Save.

<ol class="step"><li value="3">Activate MINDBODY API</li></ol>
After saving your Site Id DailyStory will display a pop-up with a MINDBODY URL and Activation Code:
	
![DailyStory + MINDBODY Activation](/articles/integrations/mindbody-02.png "DailyStory + MINDBODY Activation")

Copy either the URL or the Activation Code and use it within MINDBODY to activate API access for "DailyStory". 

Please see [this article on MINDBODY's website for more details on the required steps](https://support.mindbodyonline.com/s/article/Setting-up-an-API-integration?language=en_US).

## Fields DailyStory Syncs with MINDBODY
DailyStory will sync the following fields from MINDBODY:
	
* First Name
* Last Name
* Date of Birth
* Address
* City, State/Region, Country, and Zip/Postal code
* Gender
* Home Phone
* Mobile Phone
* Promotional Email Opt In (“Subscribe to our newsletter & promotions” setting checked profile)
* Client Status (Anything other than “Active”, will flag the contact in DailyStory as “Inactive”)
* Client Photo
* Client Membership
* Member Id
* First seen date

## Frequently Asked Questions
Below are some frequently asked questions.

### Why is MINDBODY integration only available with certain DailyStory licenses?
MINDBODY requires partners to pay to access their APIs for each MINDBODY Site Id. Because this is an expense for DailyStory we only offer this integration for some licenses. However, please [contact us](https://www.dailystory.com/contact-us/) as we can make exceptions.

### Does DailyStory update MINDBODY?
Currently, no. DailyStory only receives updates from MINDBODY. We may consider adding two-way sync in the future.

### How often does DailyStory sync data with MINDBODY?
DailyStory syncs data with MINDBODY every 3 hours.