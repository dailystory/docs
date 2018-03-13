{
	title: 'March 2018 Product Update',
	description: 'Product Updates for March 2018'
}
# March 12, 2018
* Library updates
* Fix bug with adding all contacts to list
* Added lookup to parse base domain
* Updated email parser loops to use HashSets instead of arrays
* Additional validation checks for emails
* Better error handling for failed writes to web tracking queue

# March 8, 2018
* Fix some build warnings
* Add better dsid checking/validation

# March 4, 2018
* Refactor Parser
* Improvements to format percentages as part of reports
* More improvements to validation checks on emails
* Changed IsDuplicate check on leads to return the duplicate Id
* Added Nurturing as a LeadStatus type
* Added LoadStringArrayFromFile to Common class

# March 1, 2018
* Better Html stripping in Common formatter
* Refine keywords for identifying service providers
* Work on email parser
* Add email validation check in case we get a CSS rule

# March 2, 2018
* Refactor email parser