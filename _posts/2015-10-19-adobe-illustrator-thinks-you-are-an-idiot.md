---
layout: post
title: Adobe Illustrator thinks you're an idiot
date: 2015-10-18 13:42:00.000000000 +01:00
categories:
- Thoughts
status: publish
type: post
published: true
meta:
  svg_header: '<svg xmlns="http://www.w3.org/2000/svg" width="156" height="156" viewBox="0 0 156 156"><path d="M0 0v156h156V0H0zm130 130H26V26h104v104z"/><path d="M52.1 104H82l8.6 17 9.9.6L72.2 52h-10l-28.7 52h18.6zM67 52.8L78.7 84H55.3L67 52.8zM112 64h9v51h-9zm4.6-10.5c3.3 0 6-2.7 6-6s-2.7-6.1-6-6.1-6.1 2.8-6.1 6.1 2.8 6 6.1 6z"/></svg>'
  tl;dr: 'Illustrator applies snapping when you create a document. Turn it off in the advanced section.'
author:
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus
    
---

I've recently found myself staring blankly at illustrator when I use pathfinder. Let me tell you why.

Lets say you have two rounded rectangles and you want to merge them together into this neat little plus sign. You highlight your shapes, like you always would:

![image](/assets/imgs/illustrator_snapping_01.png)

Head over to the pathfinder window and click on your favourite combining icon.

![image](/assets/imgs/illustrator_snapping_02.png)

Now, normally, you'd get one shape, looking exactly how you wanted it to, all perfectly joined. However...

![image](/assets/imgs/illustrator_snapping_03.png)

What the hell is that. Everything is misaligned, fucked up and just plain wrong.

## Diagnosing my ignorance

After much confusing and searching and digging, it turns out, your illustrator document is fucked from the beginning if you don't pay attention to Adobes new features.

When you're creating a digital asset, you would normally just start a new document, ignore all the features that illustrator gives you and just colour and resize it as you see fit when you're creating.

However, you'll notice in the advanced section of a new document window, at the bottom, there's a new checkbox –  __"Align New Objects to Pixel grid"__.

![image](/assets/imgs/illustrator_snapping_04.png)

This is where my advice would be to un-check it. If I wanted invisible snapping, i'll define my own grid to stick to.

![image](/assets/imgs/illustrator_snapping_05.png)

Now when you pathfind – you're as good as golden.

![image](/assets/imgs/illustrator_snapping_06.png)

Hopefully, you've not gone mad before finding this post.