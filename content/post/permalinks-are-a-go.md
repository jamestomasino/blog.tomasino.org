---
title: "Permalinks are a Go"
date: "2007-02-19"
author: "tomasino"
tags:
  - "Meta"
  - "RSS"
  - "Web Design"
slug: "permalinks-are-a-go"
---

After a weekend full of fun work with XSLT, XPath, Python, and PHP, I
figured out how to implement my permalinks like I wanted. The desired
effect was pretty simple:

1.  The permalinks should be taken from the original RSS source
2.  Only the proper article should be displayed
3.  The article should be styled just like the normal RSS page,
    theoretically using the same XSLT and/or CSS

Thanks to XPath, PHP, and SimpleXML I was able to make it work without
too many problems. In fact, I wasted most of my time trying to find a
Python solution. Unfortunately, the built-in Python XML API doesn't have
XPath support (at least not that I could find). And while there are many
Python XML libraries I could have chosen to fill in the gaps, I had a
heck of a timei trying to install them. Eventually I fell back on PHP.

I'll keep looking for more Python solutions when I have time, but this
works pretty well for now. It looks like all that is left for this blog
is a good method for doing comments. If anyone knows how other RSS feeds
handle those, please fill me in.
