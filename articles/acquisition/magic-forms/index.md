{
title: 'Magic Forms',
description: 'Integrate with existing web forms such as Eloqua, Marketo, or custom web forms.'
}
# DailyStory Magic Forms
A DailyStory Magic Form enables you to integrate DailyStory with any web form on your website. This includes custom HTML forms or those built with Marketing Automation Platforms such as Marketo, Eloqua, HubSpot and many others HTML form applications.

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F3juMDdvmohM%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D3juMDdvmohM&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2F3juMDdvmohM%2Fhqdefault.jpg&key=internal&type=text%2Fhtml&schema=youtube" width="500" height="281" scrolling="no" frameborder="0" allowfullscreen></iframe>

Use DailyStory Magic Forms when you cannot use a [DailyStory Web Form](/acquisition/web-forms/) or do not wish to use the [DailyStory API](/acquisition/web-forms/#creating-a-custom-html-form) for integration.

> To use Magic Forms, the [DailyStory tracking code](/install) must be included on the page of the webform.

Once you've setup DailyStory Magic Forms for your existing HTML form, DailyStory will capture customer data, optionally pre-populate forms, and associate the identifying email address with a DailyStory record. 

DailyStory does all this without requiring any changes to your existing forms or the addition of any custom code.

## Creating and Editing a Magic Form

To creae a new Magic Form go to Acquisition > Magic Forms. There you will find a list of all the existing Magic Forms. You can edit a Magic Form by clicking on it and you can create a new Magic Form by clicking the + New Magic Form button: 

![All Magic Forms](/articles/acquisition/magic-forms/magic-forms-01.jpg "All Magic Forms")

Clicking either will open the Magic Form editor:

![Magic Form Editor](/articles/acquisition/magic-forms/magic-forms-02.jpg "Magic Form Editor")

The Magic Form editor is very simple, but does have several required fields.

**Name** The name of the Magic Form must be set. This is used mainly as a helpful reference for identiying the Magic Form.

**Url** The full URL to the page containing the existing HTML form. For example, www.dailystory.com/contact-us. The full URL, including the domain, is required.

**Campaign** The [campaign](/campaigns/) within DailyStory that new leads should be created in. When the form associated with the DailyStory Magic Form is submitted the data from the form will be used to create a new lead in this campaign.

**Enabled** The Enabled toggle controls whether or not the Magic Form is enabled. When disabled the Magic Form is paused will not collect data from your web form.

> Changes to enabled/disabled status can take up to 20 minutes to take effect.

**Form Fields** The form fields contain the mapping between your form and a DailyStory lead. For example, if you have a form field named ```C_Email_Address``` you would map it to ```Email address```.

> The Lead Email address field must be mapped to a field in your form. It is the only required form field. All other fields are optional.

Not all of your form fields will be mapped to DailyStory Magic Forms.  And Magic Forms are not meant to replace your existing automation system. Rather it provides association between a visitor and an email address and attributes the lead to the appropriate campaign.

In addition to capturing the form fields, DailyStory will also capture the unique DailyStory Id of the visitor and their IP address.

## Auto-discover Form Fields
The Magic Form editor can auto-discover your form fields. 

Simply click the Auto-discover button next to the URL and DailyStory will populate the Form fields with a list of the fields it finds. You will need to then map the discovered fields to the corresponding DailyStory lead fields.

> Auto-discover will not work with all forms. For example, Marketo forms are generated dynamically with JavaScript and the fields must be manually added.

## Add Form Fields
If Magic Forms cannot auto-discover your form fields, you will need to add them yourself.

Type the name of the form field - this corresponds to the ```name``` value of a form element. For example, this form element ```<input type="text" name="FirstName">``` has a name field of ```FirstName```. Next, select the appropriate DailyStory Lead field to map ```FirstName``` to, e.g. ```First name```.

## Known Issues
Magic Forms require that the form uses an ```<input type="submit">``` button. We intend to add support for other form submit options in the future.

We occassionally encounter forms that do not work with DailyStory Magic Forms. If your form does not work, [please let us know](https://www.dailystory.com/contact-us) and we'll see about adding support.