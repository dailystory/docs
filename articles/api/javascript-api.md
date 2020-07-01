{
	title: 'DailyStory JavaScript API',
	description: 'Documentation for DailyStory\'s JavaScript API'
}
# DailyStory JavaScript API
The [DailyStory Track Tag](/install) adds activity tracking, but it also loads the DailyStory JavaScript API.

The DailyStory JavaScript API is a pure JavaScript class and has no dependencies on jQuery or other JavaScript frameworks.

> **Important** the DailyStory JavaScript API is loaded asynchronously. This ensures it does not interfere with your page load time, but also means that the API is not available immediately.

To ensure that the DailyStory JavaScript API is available you should run any JavaScript code that uses the API after the <code>ds_ready</code> event fires:
	
<pre class="brush: js; html-script: true">
    // Listen for the event.
    window.addEventListener('ds_ready', function (e) {
    	
        console.log('The DailyStory JavaScript API is ready')

    });
</pre>

The DailyStory JavaScript API is then accessed using the object reference <code>Ds</code>.

## Helper Functions
There are a number of helper functions available.

### Ds.getQueryString(field)
This helper function returns the value of data sent on the query string. If no value is found it return null.

<pre class="brush: js; html-script: true">

    var name = Ds.getQueryString("name");

</pre>

### Ds.loadJson(url, callback)
This helper function loads a Json object from a given url and calls a delegated function upon completion. You can also use it with an anonymous function.

<pre class="brush: js; html-script: true">

	// anonymous function
    Ds.loadJson('https://mysite.com/some.json', function(err, json) {
    	// do something here
    });

	// delegated function
    Ds.loadJson('https://mysite.com/some.json', myFunction);

	// called after json is loaded
	function myFunction(err, json) {
		// do something here
	}
    	
</pre>

### Ds.addEvent(obj, event, callback)
Ensures events are safely added for all browser types. For example, if you want to listen to the click event of a button:

<pre class="brush: js; html-script: true">

	&lt;button id="mybutton" &gt;click me&lt/button&gt;

	// add click handler to mybutton
	var button = document.getElementById('mybutton');
    Ds.addEvent(button, 'click', buttonClicked);
    
    function buttonClicked(e) {
    	console.log('The button was clicked');
    }
    
</pre>
	
### Ds.hasClass (element, className)
Checks an element to see if it contains a class name.

<pre class="brush: js; html-script: true">

	&lt;input type="text" id="myTextbox" class="error" &gt;

	// is the error class present?
	var textbox = document.getElementById('myTextbox');
	var exists = Ds.hasClass(textbox, 'error');
    
</pre>

### Ds.addClass (element, className)
Adds a class name to an element.

<pre class="brush: js; html-script: true">

	&lt;input type="text" id="myTextbox" &gt;

	// is the error class present?
	var textbox = document.getElementById('myTextbox');
	Ds.addClass(textbox, 'error');
    
</pre>

### Ds.removeClass (element, className)
Removes a class name from an element.

<pre class="brush: js; html-script: true">

	&lt;input type="text" id="myTextbox" class="error" &gt;

	// is the error class present?
	var textbox = document.getElementById('myTextbox');
	Ds.removeClass(textbox, 'error');
    
</pre>	