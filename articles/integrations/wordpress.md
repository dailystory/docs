---
layout: _ArticleLayout
title: WordPress Integration
description: Integration for DailyStory and WordPress
---
# WordPress Integration for DailyStory
DailyStory enables integration with WordPress that is simple to setup and easy to use. The integration makes use of a [DailyStory plugin for WordPress](/install/wordpress). Just install the plugin and you'll be ready to use the integration.

> The DailyStory WordPress plugin adds DailyStory visitor tracking to your WordPress website and also enables the DailyStory WordPress shortcodes.

## Shortcode Quick Reference
<table class="table">
<tbody>
<tr>
<td><strong>Shortcode</strong></td>
<td><strong> Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code>[ds-webform id="#"]</code></td>
<td>The webform shortcode is built to enable you to use DailyStory Web Forms in your WordPress pages and posts. Using this shortcode you can quickly build landing pages in WordPress and easily get that data back into DailyStory. This shortcode requires the [id of the DailyStory form](/acquisition/web-forms/#unique-id) you wish to display.</td>
</tr>
</tbody>
</table>
## Web Form Shortcode
The webform shortcode, <code>[ds-webform id="#"]</code>, enables you to use [DailyStory Web Forms](/acquisition/web-forms/) in your WordPress pages and posts.

> Important - this presumes you have the [WordPress plugin for DailyStory](/install/wordpress) already installed.

Let's look at an example for how the <code>[ds-webform id="#"]</code> shortcode is used.

<ol class="step"><li value="1">Get the Web Form Unique Id</li></ol>
First, you'll need to [create or edit a Web Form](/acquisition/web-forms/#creating-a-web-form) in DailyStory and get the Web Form's unique id:
	
![Web Form Unique Id](/articles/acquisition/web-forms/webforms-12.png "Web Form Unique Id")

<ol class="step"><li value="2">Create a Page in WordPress</li></ol>
Next, create or edit a WordPress page or post and add <code>[ds-webform id="#"]</code> where # is the id of your webform. Using the unqiue web form id value from step 1, this would be:
	
<code>[ds-webform id="a2vmy"]</code> 

<ol class="step"><li value="3">Publish the WordPress Page</li></ol>
Next, publish the page or post and view it in your browser.

When WordPress receives the request it will see the shortcode <code>[ds-webform id="a2vmy"]</code>. It will route that request to the DailyStory plugin to process. The plugin will make an API call to DailyStory, fetch the appropriate form, progressively render its layout, add javascript for validation, add stylesheets and optionally render a Google reCAPTCHA.

When your request completes you won't see <code>[ds-webform id="a2vmy"] (unless there was a problem), but you will instead see the HTML form that you designed on DailyStory. 

Submissions to that form are POSTed to DailyStory and new content is accessible in your lead queue associated with the campaign for that Web Form.

![WordPress Form](/articles/integrations/wordpress-01.png "WordPress Form")

