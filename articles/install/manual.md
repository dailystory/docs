{
	title: 'Manually install DailyStory tracking tag',
	description: 'Install the DailyStory tracking tag directly into your web page.'
}
# Manually Add The Tracking Tag
The tracking tag can be manually added to your website very easily ... as long as you are comfortable editing HTML pages. 

<ol class="step"><li value="1">Copy the tracking code JavaScript</li></ol>

Copy the [DailyStory tracking code JavaScript](/install/).

<ol class="step"><li value="2">Add to the &lt;head&gt; of your website</li></ol>
It is important that the tracking code is added on all pages. Many websites have a common header file. 

For example, in WordPress there is a header.php you can edit. Howevever, it is much easier (and safer) to use the [using the DailyStory WordPress Plugin](/install/wordpress). 

Add the tracking code between the opening and closing <code>&lt;head&gt;</code>:

<pre class="brush: js; html-script: true">
&lt;html&gt;
&lt;head&gt;
Insert your tracking code here
&lt;/head&gt;
</pre>

> If you aren't comfortable doing this <a href="https://www.dailystory.com/contact-us">we would be happy to help.</a>

We are building plugins for other popular content publishing tools and support [Google Tag Manager](/install/google-tag-manager).
