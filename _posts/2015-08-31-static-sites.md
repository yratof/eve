---
layout: post
title: Static sites.
date: 2015-08-31 13:05:54.000000000 +01:00
categories:
- Thoughts
tags: []
status: publish
type: post
published: true
meta:
  _edit_last: '1'
  svg_header: ''
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
<p>It seems that every other day, a wordpress website that I've built gets hacked. It starts sending out spam emails or injecting links into itself on every page refresh. It's getting to a point where I want an alternative.</p>
<p>I want change. I can't keep playing cat and mouse with bots, and frankly I shouldn't have to.</p>
<p>Having spent an evening exploring the concept of static websites (You know, those things we used to build), I stumbled upon something at may be the answer to some of the problems I've been having.</p>
<p>Enter <a href="http://en.staticpress.net">http://en.staticpress.net</a>, <a href="https://wordpress.org/plugins/really-static/" target="_blank">Really Static</a> and <a href="https://wordpress.org/plugins/super-static-cache/" target="_blank">Super Static</a>.</p>
<p>It's a plugin for your wordpress that generates a completely static version of your site. No databases, no PHP; just straight up HTML that you'd see on the site anyway.</p>
<p>Now, I've just ran it through the latest build of the FPD website to see what differences there are. Instantly, I've got thoughts – How does it handle contact forms?</p>
<p>Well... it doesn't. It fails to know what to do with them, and just presents you with the form as markup. My solution? Change the forms action to use this service: <a href="http://formspree.io">http://formspree.io</a>. A neat little form action for static sites. It sends all the data from the form to this site, then sends it over to your inbox. Inject this with JS when your form doesn't load and problem solved.</p>
<h2>Syncing</h2>
<p>Now the beauty of a static site lies in the version control. <code>git init</code> on the static site and you've managed to lock your whole site in it's current state to a commit. If anything goes wrong from this point onwards, you can simply roll back to this version.</p>
<p>Couple this with the hook that staticpress can send your static files to the server when you rebuild and you don't actually have to put your wordpress website live, you only have to publish the static version. Meaning you could install wordpress on a secure domain, under lock and key and hidden from robots, then every time your publish or update a post, your static site is updated via FTP.</p>
<p>Even better – github pages. Free hosting, secure, scalable. Free.</p>
<p>This solution eliminates the need for PHP or databases on your live server, cutting down hacks to a big fat 'never happened mate'. Plus the benefits of your site being faster from all that PHP you don't have to render and tables you don't have to fetch. you're left with google patting you on the back for having such a fast site. Unless you use a video header and 2000px wide images throughout...</p>
<h2>One step further</h2>
<p>So I've generated a static site from my wordpress. What else can we do to it?</p>
<p>Well, one thought that comes to mind is having a grunt file in there that can minimise html and inline images (small ones mind). This is another layer work that can be done to the site to get it loading much faster.</p>
<p>Realistically though, I could just not use wordpress and try something that is static already. But since I've got a barrel of clients that are already setup with wordpress, this would be the ideal way of getting them a little more secure.</p>
