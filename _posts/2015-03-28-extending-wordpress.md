---
layout: post
title: Extending Wordpress
date: 2015-03-28 15:44:56.000000000 +00:00
categories:
- Responsive
tags:
- plugins
status: publish
type: post
published: true
meta:
  _edit_last: '1'
  svg_header: <svg xmlns="http://www.w3.org/2000/svg" width="364.1" height="328.1"
    viewBox="0 0 364.1 328.1"><g stroke="#000" stroke-width="10" stroke-linecap="round"
    stroke-linejoin="round" stroke-miterlimit="10"><path fill="#EC634C" d="M68.8 197.4l-45.5-30.2v-45.5l45.5
    30.3zM114.2 121.7l-45.4 30.3-45.5-30.3 45.5-30.3zM68.8 197.4l45.4-30.2v-45.5l-45.4
    30.3z"/><path fill="none" d="M68.8 91.4v41.8"/><path fill="#fff" d="M55.5 143.2l13.3-10M23.3
    167.2M81.2 142.5l-12.4-9.3"/></g><g stroke="#000" stroke-width="10" stroke-linecap="round"
    stroke-linejoin="round" stroke-miterlimit="10"><path fill="#fff" d="M176.3 318l-75-50v-75l75
    50z"/><path fill="#EC634C" d="M251.3 193l-75 50-75-50 75-50z"/><path fill="#fff"
    d="M176.3 318l75-50v-75l-75 50z"/><path fill="none" d="M176.3 143v69"/><path fill="#fff"
    d="M154.3 228.4l22-16.4M101.3 268M196.8 227.4l-20.5-15.4"/></g><g stroke="#000"
    stroke-width="10" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10"><path
    fill="#EC634C" d="M68.8 151l-45.5-30.3v-45.5l45.5 30.3z"/><path fill="#fff" d="M114.2
    75.2l-45.4 30.3-45.5-30.3 45.5-30.2z"/><path fill="#EC634C" d="M68.8 151l45.4-30.3v-45.5l-45.4
    30.3z"/><path fill="none" d="M68.8 45v41.8"/><path fill="#fff" d="M55.5 96.7l13.3-9.9M23.3
    120.7M81.2 96l-12.4-9.2"/></g><g stroke="#000" stroke-width="10" stroke-linecap="round"
    stroke-linejoin="round" stroke-miterlimit="10"><path fill="#fff" d="M41.5 323.1l-36.5-24.3v-36.5l36.5
    24.3z"/><path fill="#EC634C" d="M77.9 262.3l-36.4 24.3-36.5-24.3 36.5-24.3z"/><path
    fill="#fff" d="M41.5 323.1l36.4-24.3v-36.5l-36.4 24.3zM41.5 238v33.6M30.8 279.5l10.7-7.9M5
    298.8M51.4 279l-9.9-7.4"/></g><g stroke="#000" stroke-width="10" stroke-linecap="round"
    stroke-linejoin="round" stroke-miterlimit="10"><path fill="#EC634C" d="M310.1
    278.7l-45.5-30.3v-45.4l45.5 30.3z"/><path fill="#fff" d="M355.5 203l-45.4 30.3-45.5-30.3
    45.5-30.3z"/><path fill="#EC634C" d="M310.1 278.7l45.4-30.3v-45.4l-45.4 30.3z"/><path
    fill="none" d="M310.1 172.7v41.8"/><path fill="#fff" d="M296.8 224.4l13.3-9.9M264.6
    248.4M322.5 223.8l-12.4-9.3"/></g><path fill="#fff" stroke="#000" stroke-width="10"
    stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" d="M212.7
    56.9l-15.9 144.6 109.6-50z"/><circle fill="#fff" stroke="#000" stroke-width="10"
    stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" cx="284.1"
    cy="80" r="75"/><path stroke="#000" stroke-width="10" stroke-linecap="round" stroke-linejoin="round"
    stroke-miterlimit="10" fill="none" d="M331 60.3l-94 .6M331.2 100.1l-69.3.4M248
    100.6l-9.3.1M238.6 80.7l69.3-.5M321.8 80.2l9.3-.1"/><path fill="#EC634C" stroke="#000"
    stroke-width="10" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10"
    d="M330.9 40.5l-.1-19.2c-13-10.3-29.3-16.4-47.1-16.3-17.8.1-34.1 6.4-46.9 16.8l.1
    19.2 94-.5z"/></svg>
  _svg_header: field_54cebcfc17f3a
  tl;dr: ''
  _tl;dr: field_54b2ee51e0a05
author:
  login: eve
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus

  options: {}
---
<p>There are some plugins that I find myself using constantly. These don’t always apply, but they always help me out. These plugins listed here aren’t anything that changes the design of my websites, they just help create an overall better experience for the people I’m building it for.</p>
<h2>Imsanity</h2>
<p><a href="https://wordpress.org/plugins/imsanity/">https://wordpress.org/plugins/imsanity/</a></p>
<p>Clients don’t have a clue. So why give them the ability to upload 10,000px wide images when they’re never used? This plugin caps the sizes images are uploaded at and can even go back through your old images and being then back to a normal scale. Uploading 4k images is a little too future proofing for the next ultra HiDpi screen.</p>
<hr />
<h2>Imagemagick Engine</h2>
<p><a href="https://wordpress.org/plugins/imagemagick-engine/">https://wordpress.org/plugins/imagemagick-engine/</a></p>
<p>Images are big. Don’t keep them that way. Compress them. Optimise them. Best of all, regenerate them. We all know that half way through building a site, you'll need to change a thumbnail size, this helps regenerate them and delete the old stuff you don't need.</p>
<hr />
<h2>wp-rocket</h2>
<p><a href="http://wp-rocket.me">http://wp-rocket.me</a></p>
<p>Caching at it’s finest. You don’t need all the complexities that come with the other big players in wordpress caching. This one will sort you out no end.</p>
<hr />
<h2>Advanced Custom Fields</h2>
<p><a href="http://www.advancedcustomfields.com">http://www.advancedcustomfields.com</a></p>
<p>Post Meta is amazing. How it’s presented is not. This helps create an interface that clients can actually use.</p>
<p>No more long lists of fields that bare no resemblance to what they affect; now we can tab things, order, and think about how to lay out the back end. The best part is that with version 5, all the add-ons are now built in: So galleries, repeating and flexible fields are all part and parcel of designing your admin area.</p>
<hr />
<h2>Little hippo</h2>
<p><a href="https://wordpress.org/plugins/little-hippo/">https://wordpress.org/plugins/little-hippo/</a></p>
<p>I used wordpress SEO by yeast for a while, just because it's what everyone uses right? Well, I discovered this little gem recently, and it makes ongoing SEO crap nicer. You can edit all your pages meta data on one page and categorised into something that doesn't make you want to kill yourself.</p>
<hr />
<p>This is just a quick list, because it might help someone. If you’ve got any questions find me on twitter <a href="letterspace://mention/yratof" class="mention tag">@yratof</a></p>
