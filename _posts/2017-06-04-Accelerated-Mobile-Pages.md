---
title: Accelerated Mobile Pages und Jekyll
date: 2017-06-04 00:00:00 Z
categories:
- github
- html
- open-source
- jekyll
- amp
layout: post
gists: true
---

Ich habe meine Website jetzt komplett auf [Accelerated Mobile Pages (AMP)](https://ampproject.com) umgestellt.

*Wozu AMP?*  
AMP ist von Google veröffentlicht worden, um das mobile Internet zu beschleunigen (wie der Name schon sagt). Die mit AMP-Html geschriebenen Seiten laden im Vergleich zu normalem HTML viel schneller, weil man möglichst wenige Dateien (Scripts, Stylesheets) lädt und so die Seiten kompakt hält. Außerdem werden AMP-Seiten bei Google zwischengespeichert (im AMP-Cache), wodurch sie fast auf Klick geladen haben.
Man sieht bei Google AMP-Seiten im News-Rondell und bei Google Shopping. Bing und Twitter unterstützen AMP, sowie Tumblr, Ebay und viele andere Firmen stellen ihre Inhalte über AMP bereit.

Da ich gerade bei Projekten mit AMP, in Verbindung mit [Jekyll](http://jekyllrb.com) arbeite, wollte ich meine persönliche Webseite auch umstellen.

Damit mein Jekyll-Blog AMP unterstützt, muss das Layout angepasst werden, sowie einige HTML-Tags mit den AMP-Äquivalenten ausgetauscht werden.

Mein default-Layout (im Ordner `_layouts`) bei Jekyll sieht jetzt so aus:  

<amp-gist data-gistid="ab8e997dbaa0e13b9c884d4570d9d7c7" layout="fixed-height" height="250"></amp-gist>

[Gist default.html](https://gist.github.com/lukas-h/ab8e997dbaa0e13b9c884d4570d9d7c7)  

In der Konfigurationsdatei von Jekyll (`_config.yml`) sind mehrere Html-Tags, die durch AMP-Html-Tags ersetzt werden sollen, deklariert:

<amp-gist data-gistid="206b05564fcb15fdcbc8a438019fea8e" layout="fixed-height" height="250"></amp-gist>

[Gist: _config.yml](https://gist.github.com/lukas-h/206b05564fcb15fdcbc8a438019fea8e)

Im default-Layout werden dann mit dem [String-Filter `replace`](https://help.shopify.com/themes/liquid/filters/string-filters) bei `content` die entsprechenden Html-Tags ersetzt (wie man im ersten Code-Snippet sehen kann). 

Im default-Layout findet man die Zeile `include head.html`. Damit wird das Template für den Html-Kopf eingebunden, welches so aussieht:

<amp-gist data-gistid="4765166053040d59e51f888118333b0c" layout="fixed-height" height="250"></amp-gist>

[Gist head.html](https://gist.github.com/lukas-h/4765166053040d59e51f888118333b0c)  

In dem Code-Snippet kann man sehen, dass AMP keine externen CSS-Dateien erlaubt. Stattdessen verwendet man ein inline-`style`-Tag mit dem Attribut `amp-custom` für alle CSS-Regeln.
Wichtig ist zudem, die AMP-Javascript-Datei zu laden (`<script async src="https://cdn.ampproject.org/v0.js"></script>`).

Um noch zusätzliche [AMP-Komponenten](https://ampbyexample.com/#components) verwenden zu können, kann man in das Front-Matter der Seiten eine Variable deklarieren, in der die Script-Dateien für die Komponenten sind. Im HTML-Kopf wird dann gecheckt ob die Variable (hier `custom_elements`) vorhanden ist und somit in die Seite eingebunden wird.





Normalerweise verwendet man AMP nur, um bestimmte Teilbereiche der Website wie News-Artikel oder Produkte bei einem Onlineshop zu 'beschleunigen'.

Wenn man nur AMP-Versionen der Posts bei Jekyll erstellen möchte und **ohne** Github-Pages arbeitet, kann man den Plugin [jekyll-amp](https://github.com/juusaw/amp-jekyll) benutzen.

Wenn man nur AMP-Versionen der Posts haben will (ohne die 'unbeschleunigten', normalen Versionen), kann man ein ähnliches Layout, wie hier im Artikel gezeigt, nur für die Posts (also als Datei `_layouts/post.html`) erstellen.

update: Support für Github Gists hinzugefügt ([Gists in AMP einbinden](https://ampbyexample.com/components/amp-gist/))  
update2: Support für zusätzliche AMP-Komponenten

*Mehr* zu AMP  
[Bilderkarussell (amp-carousel) mit AMP und Jekyll
](http://himsel.me/06-12-2017-bilderkarussell-amp-carousel-mit-amp-und-jekyll.html)  
[https://ampbyexample.com](ampbyexample.com)  
[AMP Jekyll Theme](https://github.com/ageitgey/amplify)