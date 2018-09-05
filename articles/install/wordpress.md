{
	title: 'WordPress Installation Guide',
	description: 'Installing the DailyStory tracking code in WordPress.'
}
#Install DailyStory Tracking Tag in WordPress.
Installing the tracking tag in WordPress is very simple. You don't need to know PHP (that's the language/framework WordPress is written in) and you don't need to worry about trying to edit files within WordPress. Yes, we took care of all of that! All you need to do is have administrative rights to your WordPress site, an active DailyStory account ... and about 10 minutes.

While you can [follow the steps to manually add the tag](/install/manual), we highly recommend using the WordPress plugin. It is the safest way [plus it enables additional integration](/integrations/wordpress).

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="//www.youtube.com/embed/P5hjQqR2Ivg" width="300" height="150" allowfullscreen="allowfullscreen"></iframe></div>

<ol class="step"><li value="1">Install the DailyStory WordPress Plugin</li></ol>

First, install the DailyStory WordPress plugin. To do this you will need to login to your WordPress website using an account that has access to the admin area. This is usually accessible by adding /wp-admin/ at the end of your URL.

If you aren't sure what this is or haven't done that before, just tell the person or team that setup your WordPress site that you need to install the DailyStory plugin and to follow this instructions on this page. We'd be happy to help too.

Once you are in your WordPress admin area, click the menu option on the left that says Plugins. You should see the menu expand and a list of installed plugins on the right:

![WordPress Plugins](/articles/install/wordpress-01.png "WordPress Plugins")

Next, click 'Add New' in the Plugins menu on the left. This brings up another screen on the right with two options for installing plugins:

![WordPress Plugins](/articles/install/wordpress-02.png "WordPress Plugins")

Type DailyStory into the 'Search plugins...' text box. This will return a list of any plugins that have the word 'DailyStory'. It will also do a check to ensure that the plugin is compatible with the version of WordPress you are running

The DailyStory plugin should look similar to this:

![DailyStory WordPress Plugins](/articles/install/wordpress-03.png "DailyStory WordPress Plugins")

Next, click the 'Install Now' button.

<ol class="step"><li value="2">Get Your DailyStory Site Id</li></ol>

The DailyStory plugin requires your DailyStory Site ID.

The DailyStory Site ID is a unique id that lets DailyStory know who you are. You'll see it used any time you are performing any integration or APIs calls for DailyStory.

Go to the [Tracking Code page](/install) where you can find your Site ID.

Copy the code shown in the Site ID text box. We'll use this to enable the plugin:

![DailyStory Site Id](/articles/install/siteid-01.png "DailyStory Site Id")

> Note, if you don't have a DailyStory account, but want to try out our WordPress plugin - you can always [start a free 30-day trial](https://www.dailystory.com/trial).

<ol class="step"><li value="3">Activate the WordPress Plugin</li></ol>

Once you have a DailyStory Site ID you can activate the plugin.

Go back to WordPress > Plugins, activate the plugin and then click 'Settings' to configure the DailyStory plugin settings. Finally, enter the DailyStory Site ID and click 'Save Settings':

![Activate Plugin](/articles/install/wordpress-04.png "Activate Plugin")
