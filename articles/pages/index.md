{
title: 'DailyStory Pages',
description: 'Create web pages managed by DailyStory'
}
#DailyStory Pages
DailyStory Pages enable you to create stand alone micro-sites and web pages hosted on DailyStory. This is perfect for quickly building squeeze pages, landing pages, thank you pages or any other type of web page.

Unless you configure a [custom subdomain](https://docs.dailystory.com/install/subdomain) all content hosted by DailyStory is hosted on the shared domain pages.dailystory.net. Pages hosted on this domain will require a <code>_UID</code> query string parameter. Pages hosted on your own subdomain do not require the <code>_UID</code> query string parameter.

> We recommend configuring your own dedicated sub-domain, e.g. pages.example.com for hosting your content.

## Creating your first page
Creating a page in DailyStory is very simple. Just follow the steps below after navigating to Content > Pages.

<ol class="step"><li value="1">Create a page</li></ol>
After navigating to Content > Pages, click the + New Page button:

![New Page](/articles/pages/pages-01.png "Create a page")

This will open the page editor. 

<ol class="step"><li value="2">Select a campaign</li></ol>

You will be required to either select the [campaign](https://docs.dailystory.com/campaigns/) this page belongs to or create a new campaign.

![Select campaign](/articles/pages/pages-02.png "Select campaign")

Selecting a campaign tells DailyStory to attribute visitors to this page towards the statistics of the campaign. DailyStory uses this to calculcate conversion rates for the campaign.

<ol class="step"><li value="3">Title and page slug</li></ol>
Once the page editor is loaded, set a title for your page.

![Set the title and slug](/articles/pages/pages-03.png "Set the title and slug")

If this is a new page the slug for the URL is dynamially updated as you type. And if you have configured a [custom subdomain](https://docs.dailystory.com/install/subdomain) you will see it as part of the URL. Otherwise you will see a DailyStory provided subdomain.

> After editing the title the URL for the page is dynamically built. If the slug for the page already exists you will receive an error message and will be prevented from saving the page until a unique slug is used.

![Existing page slug](/articles/pages/pages-04.png "Existing page slug")

After editing the title, you can write content in the content editor.

<ol class="step"><li value="4">Page content</li></ol>

The content editor is a WYSIWYG editor. Simply write content and use menu options from the toolbar, or keyboard shortcuts, to set headers, insert images, add links, set colors, and more.

![Content editor](/articles/pages/pages-05.png "Content editor")

<ol class="step"><li value="5">Save and publish</li></ol>

Save the page and click on the permalink at the top to open it in a new browser window.

![Published page](/articles/pages/pages-06.png "Published page")

The page automatically includes the [DailyStory tag](https://docs.dailystory.com/install/) and Google Analytics (if configured).

## Advanced Page Configuration

In addition to creating a basic page using the WYSIWYG editor, you can also edit HTML and add custom CSS and JavaScript.

### Edit Page HTML

To edit the HTML of you page, click the HTML tab.

![Edit page HTML](/articles/pages/pages-07.png "Edit page HTML")

> The HTML content is automatically inserted in the &lt;body/&gt; of the page.

### Custom Head Content

If you want to add style sheets, additional meta tags, JavaScript libraries or other content you can add the HTML in the Custom Headers section.

For example, if you want to use the Bootstrap Framework for building responsive mobile pages in DailyStory, just add the Bootstrap files.

![Customize page headers](/articles/pages/pages-08.png "Customize page headers")

Now Bootstrap's CSS rules update how our page is displayed.

### Set Custom CSS Rules

You can add your own style sheet rules to the page by entering CSS in the Custom CSS editor.

For example, to set the font size of the &lt;h1&gt; tag.

![Customize page styles](/articles/pages/pages-09.png "Customize page styles")

### Add Content to the Footer

Similar to the Custom Header Content, you can add content to the footer of your page. This content will be added directly after the body content from the WYSIWYG editor and before the closing &lt;/body&gt; tag.

## Setting a Page Template

A [Page Template](https://docs.dailystory.com/pages/pagetemplate) enables you to create a reusable layout for your pages.

The Page Template is required to contain a <code>\*|BODY|\*</code> merge tag and may optionally contain <code>\*|TITLE|\*</code> and <code>\*|FORM|\*</code> merge tags.

To select a page template, choose a template from the available list of Page Templates:

![Select a Page template](/articles/pages/pages-11.png "Select a Page template")

> Once the page is saved and refreshed the applied Page Template will be visible in the WYSIWYG content editor.

When a Page Template is in use, the Page and Page Template are merged together as one when the page is requested. The <code>\*|BODY|\*</code> in the Page Template is replaced with the content of the page.

![Page template](/articles/pages/pages-10.png "Page template")

If a <code>\*|TITLE|\*</code> merge tag is found in the Page Template, it is replaced with the name of the Page. For example, this could be used to set a header in the page template: <code>&lt;h1&gt;\*|TITLE|\*&lt;/h1&gt;</code>

> It is also possible to use a <code>\*|FORM|\*</code> merge tag in a Page Template.

## Building Landing Pages

A Landing Page is a page that contains a form and is used to convert a visitor into a lead.

Landing pages are most often used along with an offer or request for information. Visitors are driven to this page from advertisements or from offers embedded in other pages.

> *What is a squeeze page?* a squeeze page is a type of landing page. A typical use for a squeeze page would be in a blog post that includes a link to a downloadable content item, such as a PDF. To receive the referenced PDF, the visitor would first need to complete a form.

To build a Landing Page you will first need to [create a form](https://docs.dailystory.com/acquisition/web-forms/) in the same campaign that the page is in.

Once you've created a form, the form will be available in the available list of Web Forms:

![Select a Page template](/articles/pages/pages-11.png "Select a Page template")

Select the form you wish to use and then use the <code>\*|FORM|\*</code> merge tag to place the form in your page.

When a Web Form is selected and placed in your page using the <code>\*|FORM|\*</code> merge tag, DailyStory will build the form and insert it into when the page is requested.

![Form in a landing page](/articles/pages/pages-12.png "Form in a landing page")

If you build multiple landing pages for the same campaign, each page can use the web form associated with the campaign.

> Web Forms can be modified independent of the page. Changes made to the form, such as which fields to include, do not require modifications to the pages using the form.

## Frequently Asked Questions

Below are some frequently asked questions about DailyStory Pages.

### Can I upload images?
Yes, you can upload images in the WYSIWYG editor. Images are publicly accessible.

### Can I include JavaScript in a page?
Yes, add JavaScript between &lt;script/&gt; blocks in either the Custom Head or Custom Footer section of your Page or Page Template.

You can also reference JavaScript files by including a link to the file in the Custom Head section.

### What is the _UID query string parameter?
The <code>_UID</code> querystring parameter is required on any pages hosted on any of DailyStory's shared domains. 

The <code>_UID</code> parameter is used to tell DailyStory which tenant the content is for. When creating a new page the preview link will contain the <code>_UID</code> parameter. 

The <code>_UID</code> parameter is not required for custom subdomains.

### What is a page slug?
A page slug is the unique name of the page following the host name. 

For example the page slug for <code>https://pages.example.com/hello-world</code> is <code>hello-world</code>. 

The slug for each page must be unique. You will receive an error if the slug is not unique and will be prevented from saving the page until it is changed.