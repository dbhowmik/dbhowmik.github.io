---
title: jekyll excerpt-separator für collections und pages
date: 2017-05-01 00:00:00 Z
categories:
- jekyll
- github
layout: post
gists: true
---

Bei Jekyll gibt es sogenannte Excerpt-Separatoren, die man für Posts festlegt um den ersten Absatz des Textes zu bekommen. Dies kann im Markdown beispielsweise eine Trennlinie wie `---` sein. Leider ist dieses Feature nur für Posts verfügbar und nicht für Collections.
Mit ein bisschen Liquid-Tricks kriegt man das zum Glück auch für Collections und andere Pages hin:

<amp-gist data-gistid="75081c62afa85dafbdc18a5bcb1242e1" layout="fixed-height" height="250"></amp-gist>

[Gist](https://gist.github.com/lukas-h/75081c62afa85dafbdc18a5bcb1242e1)