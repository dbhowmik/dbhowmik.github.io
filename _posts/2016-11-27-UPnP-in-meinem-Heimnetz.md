---
title: uPnP/DLNA zuhause
date: 2016-11-27 20:00:00 Z
categories:
- project
- uPNP
- smart-home
layout: post
---

Wer einen Raspberry Pi oder ähnliches zuhause noch in der Ecke liegen hat, kann damit wunderbar seine altmodische Stereoanlage mit Klinke internetfähig machen. Zuhause habe ich so meine Anlage aufgewertet. Im Zusammenspiel mit meinem Medienserver funktioniert das wunderbar.  
Mehr über [uPnP (Wikipedia)](https://de.m.wikipedia.org/wiki/Universal_Plug_and_Play).


Auf den Pi hab ich den uPnP-Renderer [gmrender-resurrect](https://github.com/hzeller/gmrender-resurrect) installiert. Auf der Projektseite wird super erklärt, wie man das Programm zum laufen bringt ([Link](https://github.com/hzeller/gmrender-resurrect/blob/master/INSTALL.md)) - deshalb überspringe ich die Beschreibung.
Wenn der Minicomputer mit dem LAN verbunden ist und der Stecker für die Anlage auch arretiert ist, kann man loslegen.

Wenn man nur Musik vom Smartphone aus abspielen möchte, reicht ein einfacher uPnP-Control-Point wie BubbleUPnP. Für Linux gibt es z.B. [GUPnP](https://wiki.gnome.org/Projects/GUPnP). Auf Debian kann das mit dem folgenden Befehl einfach installiert werden.  
`apt-get install gupnp-dlna-tools gupnp-tools`

Um auch größere Musiksammlungen zu verwalten, gibt es uPnP-Server. Wenn man eine Fritzbox besitzt, kann man diese als Medienserver wunderbar einsetzen; einfach Festplatte per USB anschließen, in den Adminbereich des Routers `http://fritz.box` und unter *Heimnetz > Mediaserver* ein Häkchen bei `Mediaserver aktiv` setzen.  
Eine andere Möglichkeit unter GNOME (bspw. bei Debian) ist [Rygel](https://wiki.gnome.org/Projects/Rygel). In den Systemeinstellungen können bei dem Unterpunkt *Freigabe* Ordner zur Freigabe ausgewählt werden. Über den Control-Point kann dann der Server oder Ort der Musik ausgewählt werden sowie das Wiedergabegerät.