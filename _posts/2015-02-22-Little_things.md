---
layout: post
title: It's the little things
---

####The xhtml gotcha

So after playing around a little with the epub template I downloaded, I ran it through the [epub validator](http://validator.idpf.org/ "idpf epub validator"), and received a bunch of "expected end tag" errors. After looking up the referenced lines, the only tags I found were `<br>` tags, which aren't closed. I removed them anyway, just to see what happened. **Surprise!** No errors.

The heck?

So I went to an [html reference](http://www.w3schools.com/tags/tag_br.asp "w3schools html reference") to try to figure out what's going on. And scrolling through the page, I see a header, "Differences Between HTML and XHTML". And it turns out, xhtml requires a properly closed break tag, like so: `<br />`. 

I wonder how many other differences I'm going to run into.

It appears all tags require closing. Just ran into the same issue with `<img>`.

Onward to making tiny changes one at a time, see if they do what I expect, and then change them again. Yay, iterative learning!