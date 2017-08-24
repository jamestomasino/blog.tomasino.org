---
title: "Styles and Translation"
date: "2007-02-17"
author: "tomasino"
tags:
  - "Meta"
  - "RSS"
  - "Web Design"
slug: "styles-and-translation"
---

While I mentioned before that I didn't want to build a whole GUI on top
of this blog, I was also a bit disapointed in the default rendering if
someone were to look at the xml directly. The major browsers are very
inconsistent in how they show the data. Some allow it to just show up as
plain XML. Others have built in RSS readers, now, that are hard to get
around. So I chose the solution of styling the RSS feed with an
XML-Stylesheet and some CSS. In this way, I didn't have to build any
extra technology wrappers around the feed. It works exactly the same
from all RSS readers, but now it also looks pretty if viewed in a web
browser.

Web browser support is still inconsistent, but I'm working on it. The
blog shows up properly in Firefox 1.5 and 2.0, and Opera. If you disable
your overpowering RSS reader built into Safari, it renders properly
there as well. I'll be testing IE in a bit. Next I need to make an xslt
that renders the permalinked pages. Then comments!
