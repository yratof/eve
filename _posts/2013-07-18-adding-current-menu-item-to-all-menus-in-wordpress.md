---
layout: post
title: Adding Current Menu Item to all menus in WordPress
date: 2013-07-18 11:37:00.000000000 +01:00
categories:
- Formless
tags:
- current menu item
- current page
- footer
- menus
- widgets
status: publish
type: post
published: true
meta:
  _auto_tag_removed_tags: ''
  _auto_tag_disabled: ''
  _edit_last: '1'
  wpcf-credits: https://gist.github.com/yratof/6028612
author:
  login: eve
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus

  options: {}
---
<p>Struggled with this one for a while. My main menu would do it absolutely fine, but anything in my widgets or footer or anywhere that you'd use <code>wp_nav_menu</code> wouldn't trigger the "current_page_item" class.</p>
<p>I stumbled upon this code here that you can put in your Functions.php file & it'll add a current class to all menu items that link to that page. It also leaves that class on if you go deeper into the menu, so a child or grandchild of the page will still leave that class on the 'ancestor'. Which means you can do things like show a subnav when on that page only (something that you want to do more often than not)</p>
<p><script src="https://gist.github.com/yratof/6028612.js"></script></p>
