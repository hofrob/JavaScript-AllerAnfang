---
title: jQuery
toc: 7
---
# {{ page.title }}

Eine Bibliothek die sehr viele angenehme Werkzeuge zur Verfügung stellt. Mit ihrer
Hilfe ist es nicht notwendig auf Eigenheiten spezieller Browser einzugehen. Einige
der Aufgaben, die sie erfüllt, sind:

* document ready Funktion
* Durchsuchen und Abfragen des HTML
* Verändern des HTML

## jQuery Funktion

jQuery deklariert eine Funktion die man für verschiedene Aufgaben verwenden kann.

{% highlight javascript linenos %}
jQuery();
{% endhighlight %}

Ein anderer Name für die selbe Funktion ist:

{% highlight javascript linenos %}
$();
{% endhighlight %}

Dieser ungewöhnliche Name ist möglich, da es sehr wenig Vorschriften gibt welche
Zeichen verwendet werden dürfen (im Gegensatz zu anderen Sprachen).

## document ready

JavaScript soll in den meisten Fällen erst ausgeführt werden, wenn die komplette
HTML-Seite geladen wurde (document is ready).

Um das zu erreichen gibt man der jQuery-Funktion eine anonyme Funktion (ohne Namen)
als Parameter mit. Diese anonyme Funktion wird später von jQuery aufgerufen.

{% highlight javascript linenos %}
jQuery(function() {
    alert('document is ready'); // wird als zweites aufgerufen
});

alert('document is not ready'); // wird als erstes aufgerufen
{% endhighlight %}

## HTML-Elemente abfragen

Gibt man der jQuery-Funktion einen String mit, versucht sie das Element im HTML zu
finden. Folgende Syntax ist dafür möglich:

{% highlight javascript linenos %}
jQuery('ul'); // alle unordered lists <ul>
jQuery('#logo'); // das HTML-Element mit der ID "logo"
jQuery('.nummer'); // alle HTML-Elemente mit der Klasse "nummer"
jQuery('ul#kontakte'); // <ul> Element mit ID "kontakte"
{% endhighlight %}

So eine Abfrage gibt ein jQuery eigenes Objekt zurück. Diese speziellen Objekte
stellen wiederum Funktionen zur Verfügung.

## HTML verändern

Hat man ein HTML-Element abgefragt, kann man jetzt mit der jQuery-Funktion `append()`
Daten in dieses Element einfügen.

## Übung

Erstelle mit JSFiddle in HTML ein `<p>`-Element mit einer ID.

{% highlight html linenos %}
<p id="meinText"></p>
{% endhighlight %}

Finde das HTML-Element mittels einer jQuery-Abfrage und schreibe es in eine Variable.

{% highlight javascript linenos %}
var meinText = $('p#meinText');
{% endhighlight %}

Benutze `append()` um in dieses HTML-Element verschiedene Zeichenketten einzutragen.

{% highlight javascript linenos %}
meinText.append('Hallo');
meinText.append(' .... ');
meinText.append('Welt!');
{% endhighlight %}
