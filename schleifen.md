---
title: Schleifen
toc: 9
---
# {{ page.title }}

Da wir immer wieder die selben Befehle auf ganze Arrays anwenden wollen, benötigen
wir Schleifen.

## for

{% highlight javascript linenos %}
for (var i = 0; i < kontaktListe.length; i++) {
}
{% endhighlight %}

`for` ist ein Befehl in JavaScript der eine Schleife startet. Diese Schleife
erwartet 3 Informationen.

### Zählervariable initialisieren

`var i = 0` initialisiert die Variable `i` mit dem Wert `0`. Dies wird nur einmal ausgeführt (beim Start der Schleife). Dies ist unser Zähler.

### Bedingung

Irgendwann muss diese Schleife auch wieder abbrechen. `i < kontaktListe.length` ist eine Bedingung die nach jedem Durchlauf getestet wird.

Ist sie wahr, wird der nächste Durchlauf gestartet. Ist sie falsch wird die
Schleife abgebrochen.

### Zählervariable erhöhen

Damit die Zählervariable `i` nach jedem Durchlauf erhöht wird benötigt unser
`for` eine dritte Information `i++`. Dies ist eine kurze Schreibweise von `i = i + 1`.
Dieser dritte Teil unserer `for`-Schleife wird nach jedem Durchlauf ausgeführt
(vor dem Test der Bedingung). Sie erhöht `i` um den Wert `1`.

## Übung

Die Schleife soll über unsere Variable `kontaktListe` laufen und uns mittels
`alert()` die Variable `i` anzeigen. Unser Array hat 3 Elemente. Also müssten
wir auch 3 `alert()` Fenster sehen.

## Mittels Zähler auf Array-Elemente zugreifen

Mit Hilfe der Zählervariable erhalten wir jetzt die einzelnen Array-Elemente (Objekte).

{% highlight javascript linenos %}
for (var i = 0; i < kontaktListe.length; i++) {

	var aktuellerKontakt = kontaktListe[i];

	alert(aktuellerKontakt.name);
	alert(aktuellerKontakt.nummer);
}
{% endhighlight %}
