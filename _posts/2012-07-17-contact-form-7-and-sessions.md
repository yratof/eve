---
layout: post
title: A personal Touch ~ Contact Form 7 and Sessions
date: 2012-07-17 10:35:54.000000000 +01:00
categories:
- notes
tags:
- call
- contact
- contact form 7
- forms
- intelligent
- saving
- session
- wordpress
status: publish
type: post
published: true
meta:
  _edit_last: '1'
  tmac_last_id: '258557316717244418'
  _auto_tag_removed_tags: ''
  _auto_tag_disabled: ''
  wpcf-credits: |-
    <a title="Sessions" href="http://devondev.com/2012/02/03/using-the-php-session-in-wordpress/">Sessions within WordPress</a>
    <a title="Getting data from Contact form 7" href="http://www.pushon.co.uk/blog/wordpress-contact-form-7-intelligent-thank-you-pages/">Getting formdata from CF7</a>
  dsq_thread_id: '889130852'
  _wp_old_slug: a-personal-touch-wordpress-contact-form-7-and-sessions
  _yoast_wpseo_meta-robots-adv: none
  _yoast_wpseo_sitemap-prio: '-'
  _yoast_wpseo_opengraph-description: ''
  _yoast_wpseo_google-plus-description: ''
author:
  login: eve
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus

  options: {}
---
<p>I know that this might come in handy for anyone struggling to get Contact Form 7 for Wordpress to say thanks with a personal touch.</p>
<p>I know that this is covered on a few other blog's somewhere, but I've found that they all only have a snippet of code each, so I thought I'd merge it all together so you might also find solace in making it work (finally).</p>
<p>First of all, I've tested this with the latest wordpress 3.9.1 + Contact Form 7, so when I wrote this. The world was a happier place. This might change though in the future, so for the people seeing this in years to come, leave a comment with your twitter (assuming that still exists) and correct anything that's wrong.</p>
<p>Ok, So in your theme, you're going to want to open <strong>functions.php</strong>, Scroll to the absolute bottom and paste this before the closing php tag:</p>
<p><script src="https://gist.github.com/yratof/afb46c218d1c42fb0877.js"></script></p>
<p>You're going to want to change the ['your-name'] to whatever field you have in your contact form 7 that you want to display.<br />
What that does, is start a session, then saves that field to the session so you can call it back at any point while you're still in the session</p>
<p>Next, In the Plugin itself, there is an <strong>Adittional Settings</strong> text area at the bottom, in here, simple paste the 'thank you' link in the gist:</p>
<pre>on_sent_ok: "location = 'http://www.formless.me/thankyou';"</pre>
<p>Change the URL to your THANK YOU page, that way, once the form is submitted, the form will redirect to that URL.</p>
<p>Now, you've almost done.</p>
<p>Your final part is to echo the field somewhere. Personally, I'd create a template for the THANK YOU page &amp; paste this into it:</p>
<pre>Thank You, <!--?php echo $_SESSION['formdata']; ?--></pre>
<p>That should call up the <strong>first-name</strong> that i saved to the session when i submitted the form, and should display "Thank you, Andrew". you can then wrap that in tag of your choice and make it feel like your contact form really cares about you :)</p>
<p>Hope that helps someone</p>
