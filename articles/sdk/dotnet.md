---
layout: _ArticleLayout
title: DailyStory .NET SDK Documentation
description: Documentation for DailyStory's .NET SDK
---
# DailyStory .NET SDK
The DailyStory .NET SDK is an [open source library hosted on GitHub](https://github.com/dailystory/SDKs/tree/master/DotNet) used by .NET developers to integrate DailyStory's capabilities into their .NET application.

## DailyStory Web Forms
DailyStory Web Forms enable you to [create, design and manage web forms](/acquisition/web-forms/) within DailyStory. You can then include those forms within your web application to request information from visitors, such as a signing up for a newsletter. 

> A web form is part of a [DailyStory campaign](/campaigns/) and once a form is submitted the contents are used to either create a new lead within a campaign or add to an existing lead.

### How to use
To include a DailyStory Web Form in your existing ASP.NET application, follow these steps:
	
<ol class="step"><li value="1">Add the .NET SDK Library</li></ol>
Either compile the .NET SDK yourself, or use the pre-compiled <code>DailyStory.SDK.DotNet.dll</code> library included with the SDK, and include it in the \bin folder of your ASP.NET application.

<ol class="step"><li value="2">Get your DailyStory Site Id</li></ol>
Find your DailyStory Site Id, as this will be required to use the .NET SDK. You can [find your Site Id on the Tracking Code page](/install) in your DailyStory application.

<ol class="step"><li value="3">Get your DailyStory Web Form ID</li></ol>
Next, get the Unique Id of the DailyStory Web Form you want to include. You can [find your Web Form Unique Id](/acquisition/web-forms/#unique-id) by clicking on any Web Form.

<ol class="step"><li value="4">Call the WebForm API</li></ol>
Open or create an ASP.NET page and include a reference to the <code>DailyStory.SDK.DotNet</code> and render the web form using the static <code>RenderWebForm</code> method:
	
<pre class="brush: csharp">
@using DailyStory.SDK.DotNet
&lt;h1&gt;Hello world!&lt;/h1&gt;
@Html.Raw(WebForm.RenderWebForm("[Your Site Id]", "[Your Web Form Id]"))
</pre>

> Replace [Your Site Id] and [Your Form Id] with the values from step 2 and step 3.

When you run this page, you should see something similar to this:
	
![Simple Web Form](/articles/sdk/dotnet-01.png "Simple Web Form")

Next, let's add some simple style and JavaScript to improve this web form.

> Read [more details about styling your web form](/acquisition/web-forms/#styling-your-web-form)

To make things simple, DailyStory uses [Bootstrap class names](http://getbootstrap.com/) in the CSS. While not required, this means that you can quickly use the Bootstrap framework to immediately make your form responsive and adaptive (i.e., mobile friendly).

DailyStory also provides an optional JavaScript library that automatically takes care of things like [Google reCAPTCHA support](/integrations/recaptcha) (when enabled) and client-side form validation.

> Important - the optional JavaScript library provided by DailyStory [requires JQuery](https://jquery.com/).

Finally, DailyStory additionally provides some pre-built CSS files to add form validation and basic styling. These are completely optional:

<pre class="brush: csharp">
@using DailyStory.SDK.DotNet
<head>
</head>
&lt;h1&gt;Hello world!&lt;/h1&gt;
@Html.Raw(WebForm.RenderWebForm("[Your Site Id]", "[Your Web Form Id]"))
</pre>

Now our web form looks a little nicer:
	
![Simple Web Form](/articles/sdk/dotnet-02.png "Simple Web Form")