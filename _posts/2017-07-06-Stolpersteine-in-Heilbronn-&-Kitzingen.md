---
title: Stolpersteine in Heilbronn und Anderswo - Projekt für Code for Germany
date: 2017-07-06 01:00:00 Z
categories:
- html
- open-source
- open-data
- github
- project
- Sprache
gists: true
images:
- https://opendata-heilbronn.github.io/stolpersteine-docs/uploads/startseite.png
- https://opendata-heilbronn.github.io/stolpersteine-docs/uploads/karte.png
- https://opendata-heilbronn.github.io/stolpersteine-docs/uploads/stolperstein.png
- https://opendata-heilbronn.github.io/stolpersteine-docs/uploads/aktionen.png
layout: post
---

In den letzten Monaten habe ich im Rahmen des OKLabs und in Zusammenarbeit mit dem Stadtarchiv in Heilbronn eine Website für die Stolperstein-Aktion in Heilbronn (HN) gebaut.  

Stolpersteine sind Denkmäler für Opfer (meist jüdischer Abstammung) des Nazi-Regimes. Die in den Boden eingelassenen Gedenktafeln zeigen Informationen über die Schicksale der Menschen. Das Projekt wurde von dem Künstler Gunter Demnig gestartet.

In vielen Städten Europas wurden Stolpersteine verlegt, auch zahlreiche in Heilbronn, wo das Projekt vom Stadtarchiv (Peter Wanner) koordiniert wird.

Als Teil der Initiative [Code for Germany (HN)](http://codefor.de) ist die Website für die Stolpersteine in HN entstanden. Die Heilbronner Denkmäler waren zwar davor schon im Internet vertreten, aber nicht ganz zeitgemäß und nicht mit als offen (frei verfügbar) gekennzeichneten Daten.

Die Website kann man unter [stolpersteine-heilbronn.de](http://stolpersteine-heilbronn.de) ansehen.

### Open Data & Open Source

Die Inhalte der Seite sind komplett unter einer [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) Open Data-Lizenz veröffentlicht.  
Die Daten sind in GeoJson- und Json-Form erhältlich:  
[stolpersteine.geojson](http://stolpersteine-heilbronn.de/stolpersteine.geojson)  
[stolpersteine.json](http://stolpersteine-heilbronn.de/stolpersteine.json)  
Außerdem in Markdown-Format: [Github](https://github.com/opendata-heilbronn/stolpersteine/tree/gh-pages/_list)

Der Website-Quellcode (Layouts, CSS, usw.) steht unter den Bedingungen der MIT Lizenz:
[Github Projekt](https://github.com/opendata-heilbronn/stolpersteine/)

### Wo außer in Heilbronn wird das Projekt schon eingesetzt?
Aktuell noch nirgendwo anders, wird sich aber bald ändern.   

### Features
(Siehe Bildergalerie).  
Die Website bietet eine Kartenvisualisierung der Standorte der Stolpersteine sowie eine Listendarstellung dieser. Von dort kann man zu jedem Stolperstein einen Artikel, manchmal auch Bilder und Audio anschauen, zusätzlich sind auch die Stolpersteine mit originalen Aufschriften dargestellt.
Mehr zu den Features [hier](https://opendata-heilbronn.github.io/stolpersteine-docs/docs/2-features.html).

### Technische Umsetzung
Jekyll, Github Pages, Siteleaf

### Projekt Weiterverwendung
#### Für andere OKLabs und Stolperstein-Aktionen / Initiativen
- [Wie setze ich eine Website auf](https://opendata-heilbronn.github.io/stolpersteine-docs/docs/4-website-aufsetzen.html)
- [Inhalte einpflegen](https://opendata-heilbronn.github.io/stolpersteine-docs/docs/5-stolpersteine-einpflegen.html)
- [Dokumentation](https://opendata-heilbronn.github.io/stolpersteine-docs/docs/index.html)

### Mithelfen
Infos hier: https://opendata-heilbronn.github.io/stolpersteine-docs

Das Projekt läuft im Rahmen von Code for Germany - jeder kann auf Github oder anderem Wege beitragen.

### Links

Stolpersteine-Website für Heilbronn: [stolpersteine-heilbronn.de](http://stolpersteine-heilbronn.de).

Beispielhafte Darstellung der Stolpersteine in GeoJson-Format:

<script src="https://gist.github.com/lukas-h/2a0df5216644e4507d0d784e39db5630.js"></script>

Mehr zu Stolpersteinen auf Wikipedia:  
[Stolpersteine: Wikipedia](https://de.m.wikipedia.org/wiki/Stolpersteine)  
[Liste der Stolpersteine in Heilbronn: Wikipedia](https://de.m.wikipedia.org/wiki/Liste_der_Stolpersteine_in_Heilbronn)

### Dank an:
- Stadtarchiv Heilbronn
- [*und andere*](https://opendata-heilbronn.github.io/stolpersteine-docs/docs/1-ueber.html#Team)