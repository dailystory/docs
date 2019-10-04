{
title: 'DailyStory Pages',
description: 'Create web pages managed by DailyStory'
}
# DailyStory Pages
DailyStory Pages are used to create stand alone micro-sites and web pages hosted by DailyStory. Perfect for quickly building squeeze pages, landing pages, thank you pages or any other type of web page.

> We recommend configuring your own dedicated sub-domain, e.g. pages.example.com for hosting your content.

This guide provides a list of resources to help you get started with DailyStory pages.

**Create and Edit a Page**

* [Create a Page](#create-a-page)
* [Edit a Page's Settings](#edit-a-page)
* [Page Designer](#page-designer)
* [HTML Editor](#edit-html)
* [Preview Page](#preview)

## Create a Page<a name="create-a-page"></a>
To create an page, first navigate to Content > Pages. This will display All Pages. From here you can create a new blank page or a new page from a template: 

![All Pages](https://docs.dailystory.com/articles/pages/pages-01.png "All pages")

click the menu in the top left and click "+ Create" to create a new blank email:

![Pages Menu](https://docs.dailystory.com/articles/pages/pages-01.gif "Pages Menu")

Next, you will be taken to the Pages Settings screen. When the page opens you will first need to select the [campaign](/campaigns) the page will be associated with. 

> Later, if you want to use this page in another campaign, click 'Create a Copy'. 

After selecting a campaign, you are presented with the Create Page screen:

![Create page](https://docs.dailystory.com/articles/pages/pages-02.png "Create page")

Next, set a **Name** for your page and click the "Create Page" button to save the new page.

> DailyStory will automatically create a random URL for your page. You can customize the URL later.

You can now either <a href="#edit-html">edit the HTML</a> of the page or use the <a href="#page-designer">Page Designer</a> to build a new page.

## Edit a Page's Settings<a name="c"></a>
When an page is selected from the All Pages list, the default action is to navigate to the Page Designer. 

To edit settings, such as the Name, URL or published status of the page click on the more options button to the right of a page. This will open a list of actions available for this page.

![Edit page settings](https://docs.dailystory.com/articles/pages/pages-02.gif "Edit page settings")

## Page Designer<a name="page-designer"></a>
Clicking on a page from the All Pages list or clicking the Design Page button from Page Settings will open the Page Designer.

> While it is possible to edit the HTML of the page, we recommend only editing the HTML when creating a new page template. 

![Page Designer](https://docs.dailystory.com/articles/pages/pages-03.png "Page Designer")

The Page Designer is a drag-and-drop design canvas. To add an item to the designer canvas select a widget, such as a Text Section, by clicking and holding the mouse down and drag-and-drop it onto the design surface.

You will see a green bar that indicates where the designer will place your widget.

![Email Designer drag-and-drop](https://docs.dailystory.com/articles/emails/emails-18.gif "Email Designer drag-and-drop")

When the widget is added to the designer you can move, delete or edit the widget. Some of the design widgets have special options which will show up in place of the widgets.

The Page Designer generates HTML friendly emails based on the Bootstrap templates - these are optimized all major browsers and are mobile (responsive/adaptive) friendly.

Read more about the Page Designer in our Using the Page Designer guide (coming soon!)

## HTML and CSS Editor<a name="edit-html"></a>
While DailyStory's Pages Designer enables you to quickly build robust page, more complicated page designs typically start from an HTML base.

As an example, if you have an existing landing page design you wish to use in DailyStory the best way to start is to copy-and-paste the HTML and CSS of that landing page into a new DailyStory page's HTML and CSS. 

![Pages HTML Editor](https://docs.dailystory.com/articles/pages/pages-04.png "Pages HTML Editor")

Editing the HTML of an email is an advanced option. And, emails built with the Email Designer will initially prevent you from editing the email:

![Email HTML Locked](https://docs.dailystory.com/articles/emails/emails-20.png "Email HTML Locked")

However, you can always click "Unlock HTML Editor" to edit the HTML.

> Editing the HTML of an email built with the designer may cause the designer to no longer recognize widgets added with the designer.

### Editing CSS<a name="edit-css"></a>
While editing the HTML of an email built with the designer is not recommended, the CSS of an email may be editing with no impact to the designer.

Simply click the CSS tab and edit/modify CSS rules for your email.

**Important** when DailyStory sends your email it merges all the CSS and HTML together. The full CSS is always included in a &lt;style&gt; tag of the HTML body of your email, but DailyStory will also attempt to inline the CSS rules as well. You can preview and email and view the source to see what the fully merged HTML of the email will look like.


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

Unless you configure a [custom subdomain](https://docs.dailystory.com/install/subdomain) all content hosted by DailyStory is hosted on the shared domain pages.dailystory.net. Pages hosted on this domain will require a <code>_UID</code> query string parameter. Pages hosted on your own subdomain do not require the <code>_UID</code> query string parameter.