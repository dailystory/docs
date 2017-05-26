---
layout: _ArticleLayout
title: DailyStory PHP SDK Documentation
description: Documentation for DailyStory's PHP SDK
---
# DailyStory PHP SDK
The DailyStory PHP SDK is an [open source library hosted on GitHub](https://github.com/dailystory/SDKs/tree/master/PHP) used by PHP developers to integrate DailyStory's capabilities into their PHP application.

## DailyStory Web Forms
DailyStory Web Forms enable you to [create, design and manage web forms](/acquisition/web-forms/) within DailyStory. You can then include those forms within your web application to request information from visitors, such as a signing up for a newsletter. 

> A web form is part of a [DailyStory campaign](/campaigns/) and once a form is submitted the contents are used to either create a new lead within a campaign or add to an existing lead.

### How to include a Web Form in PHP
To include a DailyStory Web Form in your existing PHP application, follow these steps:
	
<ol class="step"><li value="1">Get the PHP SDK Class Files</li></ol>
Include the PHP Class files in your PHP application. For DailyStory Web Forms you will need the [dailystory_webform.php](https://github.com/dailystory/SDKs/blob/master/PHP/dailystory_webform.php) class file.

<ol class="step"><li value="2">Get your DailyStory Site Id</li></ol>
Find your DailyStory Site Id, as this will be required to use the PHP SDK. You can [find your Site Id on the Tracking Code page](/install) in your DailyStory application.
![DailyStory Site ID and Tracking Code page](/articles/install/install-02.png "DailyStory Site ID and Tracking Code page")

<ol class="step"><li value="3">Get your DailyStory Web Form ID</li></ol>
Next, get the Unique Id of the DailyStory Web Form you want to include. You can [find your Web Form Unique Id](/acquisition/web-forms/#unique-id) by clicking on any Web Form.

![Web Form Unique Id](/articles/acquisition/web-forms/webforms-12.png "Web Form Unique Id")

<ol class="step"><li value="4">Call the WebForm API</li></ol>
Open or create a PHP page and include the <code>dailystory_webform.php</code> class. Next, create an instance of the DailyStoryWebForm object and call it's <code>renderWebForm</code> method passing in your DailyStory Site Id and Web Form Id:
	
<pre class="brush: php">
&lt;?php
require_once('dailystory_webform.php');

// Create an instance of the web form
$webform = new DailyStoryWebForm();

// Get the web form
echo $webform->renderWebForm($siteId,$formId);
?&gt;
</pre>

> Replace $siteId and $formId are the values from your DailyStory application from step 2 and step 3.

When you run this page, you should see something similar to this:
	
![Simple Web Form](/articles/sdk/dotnet-01.png "Simple Web Form")

Next, let's add some simple style and JavaScript to improve this web form.

> Read [more details about styling your web form](/acquisition/web-forms/#styling-your-web-form)

To make things simple, DailyStory uses [Bootstrap class names](http://getbootstrap.com/) in the CSS. While not required, this means that you can quickly use the Bootstrap framework to immediately make your form responsive and adaptive (i.e., mobile friendly).

DailyStory also provides an optional JavaScript library that automatically takes care of things like [Google reCAPTCHA support](/integrations/recaptcha) (when enabled) and client-side form validation.

> Important - the optional JavaScript library provided by DailyStory [requires jQuery](https://jquery.com/).

Finally, DailyStory additionally provides some pre-built CSS files to add form validation and basic styling. These are completely optional:

<pre class="brush: php">
&lt;?php
require_once('dailystory_webform.php');

// Create an instance of the web form
$webform = new DailyStoryWebForm();

// Get the web form
$form = $webform->renderWebForm($siteId,$formId);
?&gt;
&lt;head&gt;
	&lt;script src="https://code.jquery.com/jquery-3.2.1.min.js"
            integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4="
            crossorigin="anonymous"&gt;&lt;/script&gt;
    &lt;script type="text/javascript" src="https://cms-1.dailystory.com/Scripts/ds-landingpages.js"&gt;&lt;/script&gt;
    &lt;link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"&gt;
    &lt;link rel="stylesheet" id="ds-webform-css" href="https://cms-1.dailystory.com/Content/base_webform.css?ver=1.0.2" type="text/css" media="all"&gt;
&lt;/head&gt;
&lt;h1&gt;Hello world!&lt;/h1&gt;
&lt;?php echo $form?&gt;
</pre>

Now our web form looks a little nicer:
	
![Simple Web Form](/articles/sdk/dotnet-02.png "Simple Web Form")

There are several [pre-built CSS templates](/acquisition/web-forms/#styling-your-web-form) to choose from. For example, if you want a simple horizontal form you can replace the <code>base_webform.css</code> with <code>base_webform-horizontal.css</code> and change the Web Form Layout to [Hide Form Labels](/acquisition/web-forms/#form-layout):
	
![Simple Web Form](/articles/sdk/dotnet-03.png "Simple Web Form")

#### More Examples
If you would like to see more examples please see our [PHP examples in the SDK](https://github.com/dailystory/SDKs/tree/master/PHP/examples).