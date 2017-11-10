{
	title: 'November 2017 Product Update',
	description: 'Product Updates for September 2017'
}
# November 10, 2017
* Refactor popups
* Better log handling to prevent log flooding
* Better ordering for link quick menu items
* Fix HTML encoding issues with Google Analytics tag integration
* Update content pages to use Google Analytics tags and remarketing tags

# November 9, 2017
* Updated all jobs to use connection provider environment variables
* Added more tests for jobs
* Move automation rules processing to its own job
* Added RunAutomations job
* Better exception handling/logging for Salesforce
* Changed Salesforce sync to only occur on lead creation
* Fix for OriginAS parsing in Ip lookup
* Added additional logging for application errors
* Added caching for campaign rule sets as part of performance improvements
* Performance improvments to DsJsonWrapper to prevent cache race condition
* Performance improvements to WebForm lookups
* Better logic for output caching of json and other downstream file types
* Some UX improvements

# November 3, 2017
* Updates to Daily Digest
* Added form type to Web Forms to support data entry use case
* Refactor Lead to removed description from extended properties
* Refactor Lead to use Lead Extended Properties
* Added Admin class
* Added Page Info report and fixed bug in summary report
* Performance improvement to rendered json
* Performance improvements on generated Ds files

# November 2, 2017
* Remove modal campaign selector from link tracking

# November 1, 2017
* Update to Salesforce integration to better support lead field mapping
* Added SalesforceFieldItem to represent the salesforce field data
* Converted Salesforce import to use field item
* Removed some forced properties from the Salesforce object
* Added page for configuring Salesforce settings to App
* Added better support for radio and checkbox input types in Magic Forms
* Added Ux to Lead Detail for extended properties
* Added test link option to inbound/outbound links
* Formatting on IpInfo
* Updates to Lead Queue Item to write into Lead Extensions
* Added clean up to ds_redirect_log to clean up orphaned items
* Fix for Lead Extended Properties