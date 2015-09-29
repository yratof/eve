---
layout: post
title: Block semalt so it doesn't mess up your Google Analytics
date: 2014-06-06 21:37:55.000000000 +01:00
categories:
- notes
tags: []
status: publish
type: post
published: true
meta:
  _yoast_wpseo_linkdex: '65'
  _edit_last: '1'
  wpcf-credits: ''
  _yoast_wpseo_focuskw: Semalt
  _yoast_wpseo_title: How to Block semalt so it doesn't mess with Google Analytics
author:
  login: eve
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus

  options: {}
---
<p>Everytime I log into Google Analytics, I'm constantly bombarded with this URL at the top of all my results:</p>
<p><a href="http://formless.me/wp-content/uploads/2014/06/Screen-Shot-2014-06-06-at-22.30.57.png"><img class="alignnone wp-image-190 size-medium" src="/assets/imgs/Screen-Shot-2014-06-06-at-22.30.57-300x268.png" alt="Fucking Semalt" width="300" height="268" /></a></p>
<p>I mean, as confusing as Google Analytics, it's even harder to understand where the fuck anything is coming from when this SEMALT is always showing up. Now i've done a bunch of crawling on the internet myself, and it seems that semalt is a crawling referral nasty thing.</p>
<p>So we should remove it right? Well, I can't see a reason to not block it. If no real human traffic is hitting your website from this address, then you've got no reason to have it mess with your statistics.</p>
<p>To stop it from getting to your websites, put this is the .htaccess file that is in the root of your website.</p>
<p><script src="https://gist.github.com/yratof/dc99b3ece813c1c38610.js"></script></p>
<p>Source: http://codex.wordpress.org/Combating_Comment_Spam/Denying_Access</p>
