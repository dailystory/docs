---
layout: _ArticleLayout
title: WordPress Integration
description: Integration for DailyStory and WordPress
---
# WordPress Integration with DailyStory

# WordPress Plugin
The DailyStory WordPress plug does two things:

1. It automatically adds the tracking code to every page within your WordPress site. With the tracking code installed you will receive insights into what prospective customers are doing on your site. It also adds the ability for you to easily inject A/B testing of content, display exit intent or other popups and helps manage the page triggers and workflow scoring (with more to come).
2. The WordPress plugin also adds support for embedding DailyStory behavior into your WordPress pages or posts using shortcodes. WordPress shortcodes enable you to easily add functionality when writing content.

# Shortcodes
<table class="table">
<tbody>
<tr>
<td><strong>Shortcode</strong></td>
<td><strong> Description</strong></td>
</tr>
<tr>
<td width="25%"><code>[[ds-webform id="#"]]</code></td>
<td>The webform shortcode is built to enable you to use DailyStory WebForms in your WordPress pages and posts. Using this shortcode you can quickly build landing pages in WordPress and easily get that data back into DailyStory. Once the form is submitted DailyStory runs it through its workflow engine. This shortcode request the id of the DailyStory form you wish to display.</td>
</tr>
</tbody>
</table>

Let's look at an example for how the [[ds-webform]] shortcode is used.

SHORTCODE EXAMPLE

* Create or edit a WordPress page or post and add [[ds-webform id="#"]] where # is the id of your webform.

* Next, publish the page or post and view it in your browser.

* When WordPress receives the request it will see the shortcode [[ds-webform id="#"]]. It will route that request to the DailyStory plugin to process. The plugin will make an API call to DailyStory, fetch the appropriate form, progressively render its layout, add javascript for validation, add stylesheets, optionally render Google reCAPTCHA and render any call-to-action buttons.

Finally, the new HTML form replaces the shortcode and it is displayed in your browser.

When your request completes you won't see [[ds-webform id="#"]] (unless there was a problem), but you will instead see the HTML form that you designed on DailyStory. Submissions to that form are POSTed to DailyStory and new content is accessible in your lead queue associated with the campaign for that WebForm.

![WordPress Form](/articles/integrations/wordpress-01.png "WordPress Form")

