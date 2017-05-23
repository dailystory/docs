---
layout: _ArticleLayout
title: DailyStory .NET SDK Documentation
description: Documentation for DailyStory's .NET SDK
---
# Introducing the .NET SDK
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
Open or create an ASP.NET page and include a reference to the <code>DailyStory.SDK.DotNet</code>:
	
<pre class="brush: c#; html-script: true">
@using DailyStory.SDK.DotNet
</pre>

