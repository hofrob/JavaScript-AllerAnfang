---
title: Parameter von Funktionen
toc: 6
---
# {{ page.title }}

An Funktionen können Werte mitgegeben werden. Sie werden Parameter genannt und
müssen in die Deklaration dazu.

{% highlight javascript linenos %}
function eineNeueFunktion(einParameter, nochEinParameter) {
    alert();
}

eineNeueFunktion(1, 2);
{% endhighlight %}

Beim Aufruf werden die Werte in der Klammer `(1, 2)` an die Funktion mitgegeben.

Innerhalb der Funktion werden diese Werte dann den Variablen in der Deklaration zugewiesen.
Mit Hilfe dieser Variablen kann man die mitgegebenen Werte dann weiter benutzen.

## alert

`alert()` ist auch eine Funktion. Sie akzeptiert einen Parameter der dann in dem Fenster
angezeigt wird.

## Übung

Gib deiner Funktion zwei Werte mit die nacheinander mit `alert()` angezeigt werden
sollen.

{% highlight javascript linenos %}
function eineNeueFunktion(einParameter, nochEinParameter) {
    alert(einParameter);
    alert(nochEinParameter);
}

eineNeueFunktion(1, 2);
{% endhighlight %}
