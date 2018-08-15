---
title: Interview
author: Peter Baumgartner
date: '2018-08-14'
slug: interview
categories: []
tags: []
draft: yes
header:
  caption: ''
  image: ''
---

Q: Es gibt schon so viele Physikbücher warum noch eines schreiben?

A: In den USA gibt es schon eine sehr lange Tradition von Open Education Resources (OER). Und vor einigen Jahren habe ich schon englischen freie Physikbücher für das Studium und den Unterricht gefunden (z.B. „Physics for K-12“ (Sunil Kumar Singh), „People’s Physics Book“, „CK-12 Physics - Intermediate“,...). Die meisten Dokumente waren aber statische PDFs und Ergebnisse von Einzelautoren. Im deutschsprachigen Raum gab es damals etwas derartiges noch nicht. Mittlerweile hab ich auch interesannte Projekt im deutschsprachigen Raum gefunden, die mir aber nicht weit genug gehen (z.B. https://physikunterricht-online.de/).

In den letzten Jahren hat sich extrem viel getan: Web-Technologien sind gereift, Projekte wie Gitbook gestatten das Erzeugen von Dokumenten mit minimalen Aufwand, uns steht heute eine Vielzahl an freien Programm-Werkzeugen und Creative Commons Medien zur Verfügung, und Collaborative Plattformen wie GitHub und GitLab werden nicht mehr ausschließlich von Programmierern verwendet.

Im Prinzip geht es mir darum zu zeigen, was heute mit aktueller Technologie am Beispiel eines Physikbuchs für die Oberstufe möglich ist - einem _proof of concept_ - wenn man so will. Die letzten Jahre mit Linux haben mich - fürchte ich - geprägt. Die folgenden Punkte sind mir persönlich für die Umsetzung des Projekts wichtig:

- Geräteunabhängig (Smart-TV, PC, Notebook, Tablet, Smartphone, E-Book Reader, Druck)
- Betriebssystemunabhängig (Web-Browser, ePub Reader, PDF-Reader)
- Verwendung Freie Standards (HTML, JS, CSS, ePub, PDF)
- Verwendung Freier Lizenzen (CC-BY-SA 4.0, GPL 2)
- Verwendung Freier Software (Bookdown, gitbooks, R, pandoc, TeX, Inkscape,...)
- gemeinschaftlich (Alle Dateien auf Github/Gitlab)
- Freier Zugang und Respektieren der Privatsphäre (Keine Konten, keine Anmeldung, kein Tracking)
- Zeitgemäß (Volltextsuche, Teilen-Funktion,...)
- mehrsprachiger Ansatz.



Q: Du nennst dein Buch bewusst nicht Schulbuch. Was ist der Unterschied zwischen deinem Physikbuch und einem Physik Schulbuch für die Oberstufe?

A: Ein approbiertes Schulbuch muss sich immer an dem aktuellen Lehrplan und den Prüfungsbestimmungen orientieren. Es enthält kompetenzorentierte Aufgaben und Leitfäden für LehrerInnen.

Im Gegensatz dazu verstehe ich mein Physikbuch Projekt als "zweite Meinung" zum Physik-Unterricht für OberstufenschülerInnen. Es versucht Zusammenhänge so gut wie möglich - daher auch mit allen technisch möglichen Mitteln - für das mathematische Niveau eines Oberstufenschülers erklären.






Q: Du hast eine volle Lehrverpflichtung und Familie. Wie bist du auf die Idee gekommen ein solches Mammut-Projekt als Einzelperson anzugehen.

A: Zu Beginn des Projekts waren zwei Überlegungen ausschlaggebend.

Erstens sollte alles - bis auf das eigentliche Schreiben des Textes und das gelegentliche Zeichnen von Grafiken (wo ich keine passenden Inhalte auf Wikimedia Commons finden konnte) - über Programme automatisierbar sein.

Der zweite Punkt ist das Buch nicht als _mein_ Buch zu betrachten, sondern als Gemeinschaftsprojekt zu sehen. Alle Quelldateien des Projekts sollen auf eine Plattform wie GitHub oder GitLab gehostet werden und so die Hürde für die Mitarbeit von anderen Personen an dem Buch so gering wie möglich zu halten und zur Teilnahme animieren - und sei es nur die Korrektur eines Rechtschreibfehlers.

Diese beiden Ansätze sollten den zeitliche Aufwand in Grenzen halten. Soweit zur Theorie...

Zu Punkt 1: Obwohl es schon viele hervorragende freie Werkzeuge wie Pandoc und bookdown für die Erzeugung von Dokumenten und Endformaten existieren, liegt der Hund im Detail. Verwendet man z.B. Bilder von Wikimedia Commons sind in den meisten Fällen die DPI Einträge in den Metadaten falsch. Diese sind aber wesentlich für Druckausgabe. Verwende ich ein animiertes Gif Bild in der Webversion muss für die Druckversion ein bestimmter Frame gecaptured und eingebunden werden, u.s.w.
Für all diese Fälle musste ich eigens Programme schreiben, die diese Aufgaben automatisieren.

Zu Punkt 2: Im Moment herrscht noch eine ziemliche Wild West Stimmung bei dem Projekt und ich experimentiere noch viel was machbar ist. Das bedeutet aber auch, dass sich durch Programm-Code Umstellungen auch noch jederzeit Änderungen im Buch-Quelltext ergeben können. Weil ich das aber keinem anderen im Moment zumuten möchte, bleibt das Projekt vorläufig noch lokal bis sich das Framework zum Buch halbwegs konsolidiert hat.

Ich habe letztes Jahr eine 5. Klasse in Physik übernommen und versuche die Inhalte im Buch parallel zu meiner Unterrichtsvorbereitung zu verfassen, Damit meine aktuellen SchülerInnen auch schon davon profitieren. Bisher ist mir das zumeist gelungen, aber es ist zeitmäßig doch sehr aufwändig, zumal ich - leider - kein geborener Verfasser von Texten bin.





Q: Das klingt als wären die meisten Probleme gelöst. Was sind deine aktuellen Probleme?

A: Technisch ist tatsächliches schon einiges gelöst, aber die Lösungen sind vermutlich oft nicht elegant oder es gibt eine einfachere Lösung - schließlich bin ich kein Profi-Programmierer.

Ein ungelöstes Problem stellt nach wie vor das [Same-origin policy](https://en.wikipedia.org/wiki/Same-origin_policy) Sicherheitskonzept der Browser dar, die das Einbetten von Inhalten von anderen Web-Seite einschränken. Da habe ich noch keine befriedigende Lösung gefunden.

Außerdem muss noch viel Arbeit an der Dokumentation vorgenommen werden, bevor das Projekt auf github oder GitLab freigegeben wird.






Q: Erzähl etwas über deinen Hintergrund

A: Ich bin Lehrer an einem Realgymnasium in Wien und unterrichte Physik, Informatik und Mediendesign.

