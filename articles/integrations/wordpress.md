---
layout: _ArticleLayout
title: WordPress Integration
description: Integration for DailyStory and WordPress
---
# WordPress Integration for DailyStory
DailyStory enables integration with WordPress that is simple to setup and easy to use. The integration makes use of a [DailyStory plugin for WordPress](/install/wordpress). Just install the plugin and you'll be ready to use the integration.

> The DailyStory WordPress plugin adds DailyStory visitor tracking to your WordPress website and also enables the DailyStory WordPress shortcodes.

## Shortcodes
<table class="table">
<tbody>
<tr>
<td><strong>Shortcode</strong></td>
<td><strong> Description</strong></td>
</tr>
<tr>
<td width="25%" nowrap><code>[[ds-webform id="#"]]</code></td>
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

