{
	title: 'Setup a subdomain',
	description: 'Host a subdomain with DailyStory.'
}
# Steps for hosting your own subdomain with DailyStory
To enable DailyStory to host your [subdomain](https://en.wikipedia.org/wiki/Subdomain), e.g. pages.example.com, please follow the instructions below.

> *Important* You will need to talk with someone on your IT team or with your hosting company to complete these steps.

And please note, DailyStory only supports subdomains for commercial customers.

<ol class="step"><li value="1">Create a CNAME Record</li></ol>
Create a DNS [CNAME record](https://en.wikipedia.org/wiki/CNAME_record) that points to pages.dailystory.net:

<pre>
NAME                    TYPE   VALUE
--------------------------------------------------
pages.example.com.      CNAME  pages.dailystory.net.
</pre>

<ol class="step"><li value="2">Tell us</li></ol>
Once your CNAME record is configured, please tell your customer success manager. You will need to provide them with your CNAME entry, e.g. pages.example.com.

There is some network configuration that must be done by DailyStory for our servers to allow your subdomain.

<ol class="step"><li value="3">Provide a certificate</li></ol>
We *highly recommend* providing a certificate so that your pages hosted by DailyStory can be secure.

If you intend to create landing pages with forms, supplying a certificate will ensure [browsers do not show warnings](https://www.zdnet.com/article/google-tightens-noose-on-http-chrome-to-stick-not-secure-on-pages-with-search-fields/) for potentially insecure pages.

<ol class="step"><li value="4">Configure your subdomain</li></ol>
Login to your DailyStory account and navigate to Admin > Custom Subdomain under the advanced section:
	
![Custom subdomain](/articles/install/subdomain-01.png "Custom subdomain")

Enter the subdomain and a URL to redirect to if the there is a problem on the subdomain, such as when a page cannot be found.

> *Important* If you enter a URL starting with https:// you must provide DailyStory with a certificate for your subdomain.