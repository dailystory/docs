{
	title: 'DailyStory + MINDBODY ONLINE',
	description: 'Integration for DailyStory and MINDBODY ONLINE'
}
# DailyStory + MINDBODY ONLINE
The DailyStory + MINDBODY ONLINE integration enables you to use the power of DailyStory's marketing and automation tools with the [MINDBODY health and wellness platform](https://www.dailystory.com/mindbody-integration/).

When enabled, MINDBODY integration syncs MINDBODY customer data, fields, memberships, and more directly to DailyStory. Then, use DailyStory’s powerful segmentation and personalization tools to craft targeted messages for your clients.
	
> DailyStory's MINDBODY integration is only available to customers using the Professional or higher version of DailyStory.

This guide provides a list of resources to help you get started with MINDBODY integration.

**Setup Integration**

* [Configure MINDBODY integration](#configure-mindbody-integration)
* [Fields DailyStory Syncs with MINDBODY](#fields-dailystory-syncs-with-mindbody)

**Frequently Asked Questions**

* [Why is MINDBODY integration only available with certain DailyStory licenses?](#why-is-mindbody-integration-only-available-with-certain-dailysto)
* [Will DailyStory create a Contact for each of my client's?](#will-dailystory-create-a-contact-for-each-of-my-clients)
* [Can I send text messages to my clients](#can-i-send-text-messages-to-my-clients)
* [Does DailyStory update my MINDBODY contacts?](#does-dailystory-update-my-mindbody-contacts)
* [How often does DailyStory sync data with MINDBODY?](#how-often-does-dailystory-sync-data-with-mindbody)
* [Can I create segments for client's with different services or memberships?](#can-i-create-segments-for-clients-with-different-services-or-me)

## Configure MINDBODY Integration
While there are several steps required to configure DailyStory and MINDBODY integration, they are simple and don't require any technical expertise.

<ol class="step"><li value="1">Obtain MINDBODY Site Id</li></ol>
First, you need to find your MINDBODY Site Id. This is the identification MINDBODY assigns your location.

You may already know your Site Id, but if you don't, it's easy to find: when you login to your MINDBODY account, your Site Id in the url. For example:

`https://clients.mindbodyonline.com/home?studioid=-99	`

In the above URL the Site Id is `-99`.

> Your MINDBODY Site Id may be a negative number. While a little unusual, it is perfectly nornal.

Copy your Site Id and then login to your DailyStory account.

<ol class="step"><li value="2">Configure Site Id</li></ol>
Login to DailyStory and navigate to Admin > Integrations, click on the MINDBODY integration. Set the `Site Id` field with your Site Id and click Save.

![DailyStory + MINDBODY](/articles/integrations/mindbody-01.png "DailyStory + MINDBODY")

<ol class="step"><li value="3">Activate MINDBODY API</li></ol>
After saving your Site Id, DailyStory will display a pop-up with a MINDBODY URL and Activation Code:
	
![DailyStory + MINDBODY Activation](/articles/integrations/mindbody-02.png "DailyStory + MINDBODY Activation")

Copy either the URL or the Activation Code and use it within MINDBODY to activate API access for "DailyStory". This is the final step to approve DailyStory's access to your account through the MINDBODY API.

Please see [this article on MINDBODY's website for more details on the steps](https://support.mindbodyonline.com/s/article/Setting-up-an-API-integration?language=en_US) required to activate API access.

Once complete, DailyStory will automatically sync your contacts from MINDBODY.

## Fields DailyStory Syncs with MINDBODY
DailyStory will sync the following fields from MINDBODY:
	
* First Name
* Last Name
* Date of Birth
* Address
* City
* State/Region
* Country
* Zip/Postal code
* Gender
* Home Phone
* Mobile Phone
* Promotional Email Opt In (“Subscribe to our newsletter & promotions” setting checked profile)
* Client Status (Active, Non-Member, Inactive, etc.)
* Client Photo
* Client Services (any services the client is subscribed to)
* Client Memberships
* Member Id
* First seen date

The fields: Client Status, Client Services, Client Memberships and First seen date are automatically available as indexed profile fields that can be used to build segments. This is in addition to standard DailyStory contact fields that are also indexed.

## Frequently Asked Questions
Below are some frequently asked questions about DailyStory's MINDBODY integration.

### Why is MINDBODY integration only available with certain DailyStory licenses?
MINDBODY requires partners to pay to access the APIs for each MINDBODY Site Id. Because this is an expense for DailyStory, we only offer this integration for some licenses. However, please [contact us](https://www.dailystory.com/contact-us/) as we can make exceptions.

### Will DailyStory create a Contact for each of my client's?
Yes! When DailyStory runs sync for the first time, or why a new client is added to MINDBODY, DailyStory will create a new Contact record in DailyStory. Later, when information about your client changes in MINDBODY, such as they purchase a new service, this information will be added to the Contact in DailyStory.

### Can I send text messages to my clients?
Yes! Using DailyStory's [Text Messaging](/text-message) feature you can send text messages to your MINDBODY clients (as long as you have a valid mobile number).

### Does DailyStory update my MINDBODY contacts?
Currently, no. DailyStory only receives updates from MINDBODY. We may consider adding two-way sync in the future.

### How often does DailyStory sync data with MINDBODY?
DailyStory syncs data with MINDBODY every 3 hours.

### Can I create segments for client's with different services or memberships?
Yes! [Build a dynamic segment](/segments/#create-a-dynamic-segment) using a MINDBODY Service or Membership Type as part of the search criteria. DailyStory will build the segment and update it as your clients meet the criteria.