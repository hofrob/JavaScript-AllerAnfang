---
title: Chrome Developer Tools / Firebug
toc: 3
---
# {{ page.title }}

## Browser

### Chrome

In Chrome entweder

* F12
* Strg-Shift-I
* Rechte Maustaste "Element untersuchen"
* über das Menü

öffnet eine unverzichtbare Übersicht über die man verschiedene Werkzeuge erreicht.
Die beiden wichtigsten für diese Aufgaben sind "Elemente" und "Konsole".

### Firefox

In Firefox muss zuerst das AddOn "Firebug" installiert werden. Dieses kann dann über
das Käfer-Icon aktiviert werden.

## Werkzeuge

### Elemente

Zeigt den Quellcode (HTML) an den der Browser gerade anzeigt. Hier kann die Struktur
des HTML untersucht und verändert werden.

### Konsole

Hier kann JavaScript ausgeführt werden. Variablen wie vorhin beschrieben können
jetzt erstellt werden. Probier' folgendes aus:

{% highlight javascript linenos %}
var kontaktName = 'Alice';
{% endhighlight %}

Die Variable "kontaktName" ist jetzt mit dem Wert "Alice" deklariert. Den Wert
kann man jetzt abfragen indem man einfach den Variablennamen eintippt und Enter
drückt.