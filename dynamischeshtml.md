---
title: Dynamisch HTML verändern
toc: 10
---
# {{ page.title }}

Mit Hilfe von jQuery kann man HTML sehr einfach dynamisch verändern. Dafür muss man
im HTML eine Grundstruktur aufbauen die man dann zum Beispiel mit Daten befüllt.

{% highlight html linenos %}
<ul id="kontakte">
</ul>
{% endhighlight %}

In diese "unordered list" kommen jetzt Kontaktdaten die wir anfangs noch statisch
im JavaScript festlegen.

{% highlight javascript linenos %}
var kontaktListe = [
	{name: 'Amy', nummer: '99 999 9999'},
	{name: 'Fry', nummer: '88 888 8888'},
	{name: 'Bender', nummer: '77 777'}
];
{% endhighlight %}

Ein Eintrag in der Liste besteht aus dem HTML-Element "<li>" in dem Name und Nummer
des Kontakts stehen sollen.

{% highlight javascript linenos %}
for (var i = 0; i < kontaktListe.length; i++) {

	var kontakt = kontaktListe[i];

	var htmlEintrag = '<li>' + 
		kontakt.name + ': ' +
		kontakt.nummer + '</li>';

	alert(htmlEintrag);

}
{% endhighlight %}

Ist das HTML-Element korrekt erstellt, kann es in das Dokument eingefügt werden.
So wie für Text kann man dafür auch die jQuery-Funktion `append()` verwenden.

{% highlight javascript linenos %}
for (var i = 0; i < kontaktListe.length; i++) {

	var kontakt = kontaktListe[i];

	var htmlEintrag = '<li>' +
		kontakt.name + ': ' +
		kontakt.nummer + '</li>';

	$('#kontakte').append(htmlEintrag);

}
{% endhighlight %}