{
title: 'DailyStory Email Designer',
description: 'DailyStory email designer'
}
# Using the Email Designer
The Email Designer is a drag-and-drop design canvas used to more easily build and design beautiful [emails](/emails). We put together this guide to help you understand how to use the DailyStory Email Designer.

**Getting Started**

* [Overview](#overview)
* [Design Canvas](#design-canvas)
* [Widget Menu](#widgets)
* [Styling Widgets](#style-widgets)

**[Advanced Designer Topics](#advanced)**

**[Frequently Asked Quesions](#faq)**

* [Why can't I select some widgets?](#faq-cant-select)
* [How do I center an image, text or video in my email?](#faq-center)
* [Can I select my own font?](#faq-font)
* [Should I use an image as a button?](#faq-image-button)
* [Can I have an MP4 video hosted on DropBox?](#faq-mp4)
* [Can I directly embed a video into my email?](#faq-video-embed)

## Overview <a name="overview"></a>
The Email Designer has 4 main sections:

![Email Designer](https://docs.dailystory.com/articles/emails/designer-1.png "Email Designer")

1. Top menu bar - includes the name of the email, buttons and more options
2. [Design Canvas](#design-canvas) - the area where design widgets are placed
3. [Widget Menu](#widgets) - widgets that are drag-and-dropped onto the Design Canvas
4. Save buttons - buttons for saving, copying and more

### Top menu bar
The top menu bar displays the name of the email you are edting and also show contextual buttons. 

The contextual buttons shown in the top menu bar will change when widgets on the design canvas are selected.

![Email Designer](https://docs.dailystory.com/articles/emails/designer-3.png "Email Designer")

* **Select None** - When a widget is selected on the design canvas clicking Select None will unselect the widget.
* **Clear** When a widget is selected on the design canvas clicking Clear will remove the widget from the canvas.

> Important - a selected widget may also be removed by clicking the trash can or pressing the delete button.

* **Edit HTML** When a widget is selected on the design canvas clicking Edit HTML opens a popup window with the HTML for that widget.

> Important - editing the HTML of a widget is not recommended.

* **Undo** Undo a previous action, e.g. undo removing a widget from the canvas.

* **Redo** Redo a previous action, e.g. remove a widget from the canvas. 

On the far right of the menu bar you can also find the [more options button](/emails/#options).

## Design Canvas <a name="design-canvas"></a>
The Design canvas is where widgets are placed or selected.

**Selecting a widget**

When moving the mouse over the canvas a blue box will highlight widgets. To select the highlighted widget click on the widget. When the widget is selected it is outlined and a contextual toolbar is shown on the top right of the widget:

![Email Designer](https://docs.dailystory.com/articles/emails/designer-2.png "Email Designer")

Widget toolbar 

* **Up arrow** - select the parent of this widget
* **Cross arrows** - click and drag the widget to move it
* **Copy** - click to create a copy of this widget
* **Trash** - remove the widget

**Removing a widget**

A selected widget is removed from the canvas by clicking the trash icon or pressing the delete button.

> **Important** some widgets [cannot be selected](#faq-cant-select) or removed.

**Adding a widget**

To add a widget drag-and-drop it from the Widgets menu on the right. 

> if the widgets menu is not available, click "Select None".

When a widget is dragged on to the design canvas the parent widget where the widget is placed is highlighted in yellow and a green bar indicates where the widget will be placed.

![Email Designer drag-and-drop](https://docs.dailystory.com/articles/emails/emails-18.gif "Email Designer drag-and-drop")

## Widgets Menu <a name="widgets"></a>
The Widgets Menu displays design widgets that can be added to the Design Canvas by clicking, dragging and dropping to place them.

The Widget Menu display area changes when a widget is selected in the Design Canvas and has additional options.

Below is list of the widgets along with a brief description:

<table>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-text-section.png"></td>
<td style="padding-left:10px">
<b>Text Section</b><br>
The Text Section widget is used for adding text content to an email.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-image.png"></td>
<td style="padding-left:10px">
<b>Image</b><br>
The Image widget is used for adding images to an email.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-video.png"></td>
<td style="padding-left:10px">
<b>Video</b><br>
The Video widget is used for adding videos to an email. Videos from Youtube and Vimeo are supported.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-button.png"></td>
<td style="padding-left:10px">
<b>Button</b><br>
The Button widget is used for adding buttons to an email. Buttons are special HTML links with styline to display correctly in all email clients.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-content-container.png"></td>
<td style="padding-left:10px">
<b>Content Container</b><br>
The Content Container widget is used for hold other widgets or for setting background colors for sections of the email.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-divider.png"></td>
<td style="padding-left:10px">
<b>Divider</b><br>
The Divider widget is used to easily add spacing between widgets, such as two sections of text.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-email-container.png"></td>
<td style="padding-left:10px">
<b>Email Container</b><br>
The Email Container widget is a special widget used to create a 640px area where email content is added. When starting a new email in the designer, start with the Email Container.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-2-column-right.png"></td>
<td style="padding-left:10px">
<b>2 Column Text Right</b><br>
The 2 Column Text Right widget is a special widget that divides the email into 2 sections. When dispalyed on a mobile device the content on the right displays under the content on the left.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-2-column-left.png"></td>
<td style="padding-left:10px">
<b>2 Column Text Left</b><br>
The 2 Column Text Left widget is a special widget that divides the email into 2 sections. When dispalyed on a mobile device the content on the left displays under the content on the right.
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-app-store.png"></td>
<td style="padding-left:10px">
<b>App Store</b><br>
The App Store widget is a special widget that displays the iOS and Android App Store buttons using the URLs set in [Account Settings](/account/settings).
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-social.png"></td>
<td style="padding-left:10px">
<b>Social Icons</b><br>
The Social Icons widget is a special widget that displays a list of social icons with URLs set in [Account Settings](/account/settings).
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-footer.png"></td>
<td style="padding-left:10px">
<b>Footer</b><br>
The Footer widget is a special widget that displays footer content, such as address, unsubscribe, etc. set in [Account Settings](/account/settings).
</td>
</tr>
<tr>
<td style="width:120px"><img src="https://docs.dailystory.com/articles/emails/widget-comment.png"></td>
<td style="padding-left:10px">
<b>Comment</b><br>
The Comment widget is a special widget that enables you to safely add comments in emails - comments are automatically removed when the email is sent.
</td>
</tr>
</table>

### Widgets with Custom Menus
When selected, some widgets will replace the Widget Menu with options specific to that widget.

#### Text Section widget

When selected the Text Section widget opens a rich text editor in place of the Widget Menu:

![Text Section](https://docs.dailystory.com/articles/emails/designer-6.png "Text Section")

Content is written or copy/pasted into the rich editor and is updated in the Design Canvas.

> Content that is copy/pasted is stripped of any special information, such as bolding or links.

#### Image widget

When selected the Image widget opens a set of image specific options in place of the Widget Menu:

![Image widget options](https://docs.dailystory.com/articles/emails/widget-image-options.png "Image widget options")

Optionally specify if an image should be clickable. The Open File Manager button opens the DailyStory [File Manager](/file-manager) where files can be picked or uploaded.

To set the dimensions of the image, click the style tab and set the width and height.

#### Video widget

When selected the Video widget opens a set of video specific options in place of the Widget Menu:

![Video widget options](https://docs.dailystory.com/articles/emails/widget-video-options.png "Video widget options")

* **Video URL** URL to the video. When set, DailyStory will replace the default Video widget in the Design Canvas with a preview of your image.

**Supported video sources**:

* Youtube
* Vimeo

## Styling Widgets <a name="style-widgets"></a>
When a widget is selected the Widgets menu the Style tab is used to set style details about the selected widget.

![Widget style](https://docs.dailystory.com/articles/emails/widget-style.png "Widget style")

> The options shown in the Style menu change based on the widget selected.

* **Font family** the font used for text, e.g. Helvetica
* **Font size** the size of the font, e.g. 20px
* **Font weight** the weight of the font, e.g. bold
* **Line height** the spacing between lines, e.g. 24px
* **Color** the color of the text, e.g. #FFCC2A
* **Background color** the background color of the widget, e.g. #FFFFFF
* **Text align** the alignment of the content in the widget, e.g. center
* **Padding** the whitespace surrounding the widget, e.g. 15px
* **Width** the width of the widget, e.g. 100%
* **Height** the height of the widget, e.g. 250px
* **Min width** the minimum width of the widget, e.g. 100px
* **Min height** the minimum height of the widget, e.g. 100px
* **Max width** the maximum width of the widget, e.g. 500px
* **Max height** the maximum height of the widget, e.g. 500px

> Some style values, such as Min and Max height and width are not supported by Microsoft Outlook.

**Recommendation** when possible, use percentages to express image dimensions. This enables the [email to scale based on the size of the client](#responsive-email), such as mobile devices.

## Creating a new email using the Designer
The Email Designer is built to support working with pre-made email templates or building new emails 100% in the designer.

> If you are working with an agency and have a pre-existing HTML template for your emails. This email should be created as a new Email Template. Furthermore, HTML elements within the template can use special mark up to identify which HTML sections are editable and which are not.

Below is a step-by-step guide for creating a new email using only the Email Designer.

### Start with an Email Container
The Email Container widget is a widget that creates an HTML layout with a 640px center area of content optimized for mobile and desktop email clients.

An email should use multiple Email Containers to logically separate parts of the email:

* **Header** title and logo
* **Body** main content of the email
* **Footer** footer content, such as unsubscribe links

![Email sections](https://docs.dailystory.com/articles/emails/designer-7.png "Email sections")

This enables you to design an email with a colorful header area that spans the width of the email and a body and footer area that shows a white content area with a grey outter area.

## Advanced Designer Topics<a name="advanced"></a>
Below are some advanced topics related to the Email Designer.

### Image best practices<a name="image-best-practices"></a>
It's important to use images in your email, but too many images can flag your email as potential spam. And, images should be resized for optimal display in the email.

The best-practice dimension of an email is 640 px wide. If your image is wider than 640 px it means the image will have to be resized to fit in the email and the image file size is likely bigger (and will take longer to download).

* Try to strike a balance between images and text
* Resize images to 640 px width using an image editing tool
* Use percentage to specify the width of an image - this will enable the image to scale on smaller devices.

### Building mobile friendly (responsive) emails<a name="responsive-email"></a>
The majority of your email will be read on mobile devices. And, it is important to optimize the email for mobile devices.

First, ensure that for any fixed width tables, there is a CSS media query for your email so that the tables can be set to 100% width. While this won't help for Microsoft Outlook clients, your iOS and Android mobile users will be appreciative.

Second, follow [image best practices](#image-best-practices) and use images that scale. This will allow the image to resize itself automatically on smaller screens.

## Frequently Asked Questions <a name="faq"></a>
Below are some frequently asked questions about the Email Designer.

### How do I center an image, text or video in my email?<a name="faq-center"></a>
To center an Image, Text Section, or Video in your email select the widget in the designer, select the [Style Menu](#style-widgets) and set Text Align to Center. For Image and Video widgets select the Image Wrapper or Video Wrapper before centering.

### Why can't I select some widgets?<a name="faq-cant-select"></a>
Some widgets, such as HTML tables used for email layout, cannot be selected because these HTML elements are part of the underlying email template.

### Can I select my own font?<a name="faq-font"></a>
No. The fonts are currently limited to the fonts in the [Style widgets](#style-widgets) menu. This is to ensure that emails will look consistent across multiple email clients.

### Should I use an image as a button?<a name="faq-image-button"></a>
No. DailyStory's [Widget button](#widgets) is a pure HTML button designed to display across email clients. Some clients, such as Microsoft Outlook, do not display images by default. This causes images buttons to have a lower click-through rate.

### Can I have an MP4 video hosted on DropBox?<a name="faq-mp4"></a>
Yes. However, it is not supported by the Video widget. You will need to create a placeholder image that links to this video.

### Can I directly embed a video into my email?<a name="faq-video-embed"></a>
No. Email clients do not support embedded videos. When you use the DailyStory Video widget your video is replaced with an image that is linked to the video.