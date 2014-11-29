---
title: Funktionen
toc: 4
---
# {{ page.title }}

So wie Variablen, kann man auch Funktionen deklarieren. Die Syntax ist aber eine
andere.

{% highlight javascript linenos %}
function eineNeueFunktion() {
    // Inhalt der Funktion (Variablen, Aufrufe, Unterfunktionen)
}
{% endhighlight %}

Ist eine Funktion deklariert, ist das nur eine Information an den Browser, dass
es eine Funktion mit diesem Namen gibt. Sie kann später aufgerufen werden.

So ruft man eine Funktion auf:

{% highlight javascript linenos %}
eineNeueFunktion();
{% endhighlight %}

Erst durch den Aufruf werden die Befehle innerhalb der Funktion tatsächlich ausgeführt.

