---
title: Verschachtelte Variablen
toc: 8
---
# {{ page.title }}

Die verschiedenen [Variablen]({{ site.github.url }}/variablen.html) können auch
kombiniert werden. Häufig trifft man zum Beispiel auf Arrays von Objekten.

## Array mit Objekten

{% highlight javascript linenos %}
var kontaktListe = [
	{name: 'Amy', nummer: '99 999 9999'},
	{name: 'Fry', nummer: '88 888 8888'},
	{name: 'Bender', nummer: '77 777'}
];
{% endhighlight %}

Das Array "kontaktListe" hat 3 Elemente. Diese 3 Elemente sind wiederum Objekte.

Um die Struktur dieser Variable besser zu erforschen, seien hier nochmal die
[Developer Tools]({{ site.github.url }}/devtools.html) erwähnt. Die Variable
kann man in die Konsole einfügen und versuchen damit Daten abzufragen.

{% highlight javascript linenos %}
kontaktListe[0]; // {name: 'Amy', nummer: '99 999 9999'}
kontaktListe[0].name; // 'Amy'
{% endhighlight %}

## Lesbarkeit

Wichtig ist zu verstehen wie man so etwas liest. Die Variable "kontaktListe" ist
ein Array. Das heißt die einzelnen Elemente werden mit eckiger Klammer abgefragt
`kontaktListe[0]`. Dadurch erhalten wir in diesem Fall ein Objekt. Von diesem
Objekt kann man dann die einzelnen Eigenschaften abfragen `kontaktListe[0].name`.

Um die Lesbarkeit zu verbessern ist es manchmal besser das Array-Element (das Objekt)
zuerst in eine Variable zu schreiben.

{% highlight javascript linenos %}
var ersterKontakt = kontaktListe[0];
ersterKontakt.name; // 'Amy'
{% endhighlight %}

## Spezielle Eigenschaften und Funktionen von Arrays

Arrays bieten abgesehen von den einzelnen Elementen noch andere Eigenschaften und
Funktionen. Zwei häufig verwendete sind

* length
* push()

Die Eigenschaft "length" gibt die Anzahl der Elemente zurück.

{% highlight javascript linenos %}
kontaktListe.length; // 3
{% endhighlight %}

Mittels "push()" hängt man ans Ende eines Arrays ein neues Element an.

{% highlight javascript linenos %}
var neuerKontakt = {
	name: "Professor Farnsworth",
	nummer: "1 800 PLANET EXPRESS"
};

kontaktListe.length; // 3
kontaktListe.push(neuerKontakt);
kontaktListe.length; // 4
{% endhighlight %}

## Übung in der Konsole

1. Wie bekommt man das komplette erste Kontakt Objekt?
1. Wie erhalte ich die Nummer von Bender?
1. Füge einen neuen Kontakt zur Liste hinzu und kontrolliere ob die Variable korrekt
gespeichert wurde.
