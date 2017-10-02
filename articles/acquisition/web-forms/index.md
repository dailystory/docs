{
	title: 'Web Forms',
	description: 'Web forms are used to collect information about your visitors.'
}
# DailyStory Web Forms
A DailyStory Web Form enables you to quickly and easily create forms that can be shown on your website, in your mobile application, a DailyStory landing page, or elsewhere using the DailyStory API.

Creating new web forms and editing existing webforms can be found by:

* Signing in to your DailyStory account
* Navigating to Acquisition > Web Forms	
	
![DailyStory Web Form](/articles/acquisition/web-forms/webforms-01.png "DailyStory Web Form")

This opens the All Web Forms list which shows a list: 

![All Web Forms](/articles/acquisition/web-forms/webforms-13.png "All Web Forms")

Clicking on a web form will open the [Edit Web Form designer](/acquisition/web-forms/#using-the-web-form-designer). To [create a new web form](/acquisition/web-forms/#creating-a-web-form), click the '+ New Web Form' button.

## Common Questions
Below are some common questions regarding DailyStory's Web Forms.

### How do I add the web form to my existing website?
Once you've created a web form in DailyStory [you have several options for publishing it](/acquisition/web-forms/#publishing-your-web-form). The recommended method is to either use the native integration with popular CMS applications, such as [WordPress](/integrations/wordpress), or one of the SDKs ([PHP](https://github.com/dailystory/SDKs/tree/master/PHP) and [.NET](https://github.com/dailystory/SDKs/tree/master/DotNet)). These are designed to display the DailyStory web form within your site directly.
	
### What happens when the form is submitted?
When a visitor successfully completes a form the contents of the form are sent to DailyStory. The visitor is redirected to another page, typically a thank you page, that is identified as the 'Destination URL' in when [designing your web form](/acquisition/web-forms/#using-the-web-form-designer).

### What are the best practices for using web forms?
A best practice is to ensure your web form has a thank you page - this is the Destination URL when designing your web form - and that the web form sends an email to confirm receipt. Sending a thank you should also be used to validate the deliverability of the email address that the visitor provided. If the email address is invalid, you can remove them from the campaign. All of this can be configured in the [Campaign Workflow](/campaigns/#Workflow).

## Creating a Web Form
When the <code>+ New Web Form</code> button is clicked the Create New Web Form designer is opened.

The first step is to select a campaign that the web form is associated with: 

![DailyStory Web Form](/articles/acquisition/web-forms/webforms-02.png "DailyStory Web Form")

This ensures that all leads or customers that complete this web form are associated with the right campaign. 

> By associating the web form with a campaign, the campaign will be given the attribution for the lead or customer conversion.

Once the campaign is selected the Web Form Designer is available:
	
![DailyStory Web Form Designer](/articles/acquisition/web-forms/webforms-03.png "DailyStory Web Form Designer")
	
## Using the Web Form Designer	
The Web Form Designer enables you to create or edit an existing web form. Each web form requires:
	
* **A name** - a friendly name for the web form, such as Contact Us.
* **A destination URL** - where the form should send the browser once the form is completed.

The web form itself can have multiple form items, but the email address field is required and cannot be removed.

> If you attempt to remove the Email address form item an message will be shown that this form item is required and cannot be removed.

### Add / Edit Form Items
The Web Form Designer provides a simple preview of what your final web form will look like.

> This does not take into consideration any CSS applies to your web form.

Form items can be added, edited, removed and reordered using the designer.

#### Add Web Form Item
To add a web form item, click the drop down to select the type of form item to add. For example, to add a new textbox field click the Form item drop down and select textbox:

![Add form item](/articles/acquisition/web-forms/webforms-05.png "Add form item")

Next, a new form is shown

##### Textbox and Textarea
When Textbox or Textarea is selected the following options are availabe:

![Textarea form](/articles/acquisition/web-forms/webforms-06.png "Textarea form")

* Form label - this is the text shown with the form field
* Form placeholder - this is helpful text shown within the form field
* Lead field mapped to - the lead field in DailyStory to map the entered value to
* Make this required - prevents the form from being submitted unless this field is completed

Let's look an example: adding a new required form field for phone number:

![Add phone number](/articles/acquisition/web-forms/webforms-07.png "Add phone number")	

Next, we'll click 'Add form item' and this new field will be shown in the live preview:
	
![Add phone number form](/articles/acquisition/web-forms/webforms-08.png "Add phone number form")	

##### Dropdown list
DailyStory forms also support drop down lists so you can pre-define the values to be selected:
	
![Add drop down](/articles/acquisition/web-forms/webforms-09.png "Add drop down")	

> Unlike the textbox and textarea form items, there is not an option to set a form placeholder.

Drop down choices are set by entering a single option on each line. For example, if you want to ask the user to select their job title from a pre-defined list you can enter a single choice on each line. If you want to use a specific value different from the text use a comma (with no spaces):
	
![Drop down example](/articles/acquisition/web-forms/webforms-10.png "Drop down example")	

#### Edit Web Form Item
Editing a web form item is simple. Just click on the fom item to edit. It will turn yellow and the form item are displayed to the right.

![Edit form item](/articles/acquisition/web-forms/webforms-11.png "Edit form item")	

Click Update form item to save any changes and you will see this immediately reflected in the Live Preview.

#### Delete Web Form Item
Deleting a web form item is similar to editing. The only difference is that you click the Remove form item button.

### Form Options
The Form Options section enable you to change some optional settings for the web form.

#### Call to Action
The Call to Action enables you to change the text shown on the call to action button for the web form. By default this is set to <code>Submit</code>.

If you would like the call to action to be something else, such as <code>Yes, please follow-up</code>, simply enter that text here.

#### Form Layout
The Form Layout option provides you with the ability to control some layout control of the web form. While the main styling of the web form is done with CSS, you can select:
	
* Display form labels - form labels (text above the form field) will be shown.
* Hide form labels - form labels (text above the form field) will not be shown.

> While displaying or not displaying form labels can also be controlled through CSS, this setting determines if DailyStory renders the HTML itself.

#### Use reCAPTCHA
If [reCAPTCHA integration](/integrations/recaptcha) is an enabled integration you can add reCAPTCHA support to your web form.

> Provided by Google, reCAPTCHA is a free service that protects your website from spam and abuse by adding a simple test to your web or mobile experience.

The screen shot below shows an example form that includes reCAPTCHA:

![Web Form with reCAPTCHA](/articles/acquisition/web-forms/webforms-04.png "Web Form with reCAPTCHA")

### Unique Id
Once a web form is saved, or when it is edited, some additional properties about the webform are availabe. The Unique Id provides access to an id that uniquely identifies the form. This is used in the DailyStory APIs and for integrations such as [WordPress](/integrations/wordpress).
	
![Web Form Unique Id](/articles/acquisition/web-forms/webforms-12.png "Web Form Unique Id")

## Publishing your Web Form
A web form created in DailyStory can be published four ways:

* Application integration - such as the [WordPress shortcode	](/integrations/wordpress#web-form-shortcode)
* DailyStory Page - create [DailyStory Pages](/features/pages#landing-pages) that include your Web Form
* DailyStory SDK - use the [DailyStory SDK](/sdk/) to render forms in your web application
* Custom HTML form - write your own HTML and POST to the DailyStory Web Form

The table below will help you select the right option for your DailyStory Web Form.

<table class="table">
<thead>
	<th></td>
	<th>Application Integration</th>
	<th>DailyStory Page</th>
	<th>DailyStory SDK</th>
	<th>Custom Form</th>
</thead>
<tbody>
<tr>
<td><strong>Complexity</strong></td>
<td>Low</td>
<td>Medium</td>
<td>High</td>
<td>High</td>
</tr>
<tr>
<td><strong>Skill Set</strong></td>
<td>Content Developer</td>
<td>Content Developer</td>
<td>Web Developer</td>
<td>Web Developer</td>
</tr>
<tr>
<td><strong>Customization</strong></td>
<td>Limited (CSS)</td>
<td>Limited (CSS)</td>
<td>CSS & JavaScript</td>
<td>Full</td>
</tr>
</tbody>
</table>

If you have an exist web form that uses custom HTML or a Marketing Automation Platform, consider using [DailyStory Magic Forms](/acquisition/magic-forms/).

### Creating a Custom HTML form
You can also create your own custom HTML form and POST directly to the DailyStory Web Form URL. This gives you the greatest flexibility with regards to design and layout of your form.

> If you have existing forms on your website, you can easily convert your existing forms to publish to DailyStory.

To create a custom form:
	
<ol class="step"><li value="1">Configure the &lt;form&gt;</li></ol>
The &lt;form&gt; needs to be configured to POST the values to your DailyStory Web Form URL. The format of this URL is:

<code>https://cms-1.dailystory.com/PostForm/[Site Id]/[Web Form Id]</code>

For example, if your DailyStory Site Id is <code>1234567890</code> and your Web Form Id is <code>a2vmy</code> your &lt;form&gt; would look as follows:
	
<pre class="brush: js; html-script: true">
&lt;form method="POST" action="https://cms-1.dailystory.com/PostForm/1234567890/a2vmy" &gt;
</pre>	

<ol class="step"><li value="2">Add required form fields</li></ol>
DailyStory expects to find two form fields:

* DailyStory Id - form field name <code>dsid</code>
* Email address - form field name <code>Email</code>	
	
The DailyStory Id is a unique identifier used to identify customers and visitors. This hidden field is required and set to the value of the <code>_ds</code> cookie which is created as part of the DailyStory JavaScript tag.

<pre class="brush: js; html-script: true">
&lt;input type="hidden" name="dsid" value="dsid" &gt;
</pre>	

A valid email address must be included with the <code>&lt;form&gt;</code> submit and must use the <code>name</code> value of <code>Email</code>:

<pre class="brush: js; html-script: true">
&lt;input type="text" name="Email" &gt;
</pre>	
	
<ol class="step"><li value="3">Add jQuery and Landing Page Script</li></ol>
The <code>&lt;input type="hidden" name="dsid" value="dsid" &gt;</code> needs to be set to the DailyStory Id of the current visitor.

> The dsid needs to be set after the page completes loading. If the form is the first page a visitor lands on the DailyStory Id will not be written until after the page completes loading.

You can write your own JavaScript to set the value of the hidden <code>&lt;input&gt;</code> to the value in the <code>_ds</code> cookie, but the recommended way is to include jQuery and our helper library:
	
<pre class="brush: js; html-script: true">
&lt;script src="https://code.jquery.com/jquery-3.2.1.min.js"
        integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4="
        crossorigin="anonymous"&gt;&lt;/script&gt;

&lt;script type="text/javascript" src="https//cms-1.dailystory.com/Scripts/ds-landingpages.js"&gt;&lt;/script&gt;
</pre>	

<ol class="step"><li value="4">Set form field names</li></ol>
The final required step is set the form field names to match the field values supported by DailyStory.

For example, to capture the company name on a form, a form field's name must be set to <code>Company</code>.

<pre class="brush: js; html-script: true">
&lt;input type="text" name="Company"&gt;
</pre>	

A full list of the DailyStory form fields is published below.

> You can include additional custom form fields as well. The values of these fields will be available as part of the DailyStory contact.

#### Custom Web Form Lead Fields
The table below provides a list of the field name values used in a custom form that populate corresponding values in the [lead](/lead) and [contact](/contact).

<table class="table">
<thead>
	<th>Field Name</th>
	<th>Maps To</th>
	<th>Description</th>
</thead>
<tbody>
<tr>
<td>Salutation</td>
<td>Contact</td>
<td>Saluation for the contact, e.g. Mr., Mrs., Dr., Ms.</td>
</tr>
<tr>
<td>FirstName</td>
<td>Contact</td>
<td>First name of the contact.</td>
</tr>
<tr>
<td>LastName</td>
<td>Contact</td>
<td>Last name of the contact.</td>
</tr>
<tr>
<td>FullName</td>
<td>Contact</td>
<td>Full name of the contact. When set, full name will then populate first and last name.</td>
</tr>
<tr>
<td>Email</td>
<td>Contact</td>
<td>Email address of the contact.</td>
</tr>
<tr>
<td>Title</td>
<td>Contact</td>
<td>Job title of the contact, e.g. Marketing Manager</td>
</tr>
<tr>
<td>Company</td>
<td>Contact</td>
<td>Job title of the contact, e.g. Marketing Manager</td>
</tr>
<tr>
<td>NumberOfEmployees</td>
<td>Contact</td>
<td>Number of employees in the organization, e.g. 100</td>
</tr>
<tr>
<td>WebSite</td>
<td>Contact</td>
<td>Url to the company's website</td>
</tr>
<tr>
<td>Phone</td>
<td>Contact</td>
<td>Primary phone number</td>
</tr>
<tr>
<td>MobilePhone</td>
<td>Contact</td>
<td>Mobile phone number</td>
</tr>
<tr>
<td>Country</td>
<td>Contact</td>
<td>Country, e.g. United States</td>
</tr>
<tr>
<td>City</td>
<td>Contact</td>
<td>City, e.g. New York</td>
</tr>
<tr>
<td>PostalCode</td>
<td>Contact</td>
<td>Postal or zip code</td>
</tr>
<tr>
<td>Address</td>
<td>Contact</td>
<td>Address, e.g. 123 My Street</td>
</tr>
<tr>
<td>Region</td>
<td>Contact</td>
<td>Region or state, e.g. California</td>
</tr>
<tr>
<td>LeadSource</td>
<td>Lead</td>
<td>Source where the lead originated, e.g. Contact Us Form</td>
</tr>
<tr>
<td>Description</td>
<td>Lead</td>
<td>Free form text, such as reason for contacting us</td>
</tr>

</tbody>
</table>

## Styling your Web Form
