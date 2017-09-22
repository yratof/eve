---
layout: post
title: Show Products on OpenCart 404 page
date: 2014-06-16 11:17:19.000000000 +01:00
categories:
- notes
tags: []
status: publish
type: post
published: true
meta:
  _edit_last: '1'
  wpcf-credits: ''
author:
  login: eve
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus

  options: {}
---
<p>Since Opencart gives you 404's all over the place, it's nice to have customers not leave the site when they hit this brick wall.</p>
<p>I've found the best thing to do is put your products on the 404 page and lead customers back into the shop.</p>
<h2>Ok, so how do we do this?</h2>
<p>Glad you asked.</p>
<p>We're going to make a new Layout route first, so go to <strong>System &gt; Design &gt; Layouts</strong></p>
<p><img class="alignnone size-full wp-image-197" src="/assets/imgs/Screen-Shot-2014-06-16-at-12.10.39.png" alt="layouts in opencart" width="332" height="147" /></p>
<p>Then you're going to want to <strong>INSERT</strong> (which i've always wondered why it was named this, I'd rather it say add new).</p>
<p>From here, you should make the Layout name "404" so you know what the heck it is, then you're going to want to make the ROUTE</p>
<p><code>error/not_found</code></p>
<p><img class="alignnone size-full wp-image-198" src="/assets/imgs/Screen-Shot-2014-06-16-at-12.12.46.png" alt="Screen Shot 2014-06-16 at 12.12.46" width="763" height="276" /></p>
<p>Save all that and you're half way there.</p>
<p>Now you've got a way of displaying things on the 404 page, go to <strong>Modules </strong>and find what you want to display.</p>
<p>I'm going to use the Featured Module for this example. Go into it, add a new module and select 404 as your layout. Then you can add all your products and they'll show like they would if it was anywhere else on the site.</p>
<p><img class="alignnone size-full wp-image-199" src="/assets/imgs/Screen-Shot-2014-06-16-at-12.15.53.png" alt="Screen Shot 2014-06-16 at 12.15.53" width="1086" height="174" /></p>
<p>How do you feel now?</p>
