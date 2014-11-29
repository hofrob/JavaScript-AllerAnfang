---
title: Variablen
toc: 2
---
# {{ page.title }}

## Simple Variablen

Variablen müssen deklariert werden:

{% highlight javascript linenos %}
var kontaktName;
{% endhighlight %}

Es können auch mehrere Variablen auf einmal deklariert werden:

{% highlight javascript linenos %}
var kontaktName,
    kontaktNummer;
{% endhighlight %}

Zur besseren Lesbarkeit sollte jede Variable in einer eigenen Zeile stehen. Die Deklaration mit `var` endet erst beim Strichpunkt (`;`).

Bei der Deklaration können auch gleich Werte zugewiesen werden:

{% highlight javascript linenos %}
var kontaktName = '',
    kontaktNummer = '+43 ';
{% endhighlight %}

## Komplexe Variablen

### Array

Ein Array ist eine Liste von Werten:

{% highlight javascript linenos %}
var filme = [
    'M',
    'Es',
    'Up',
    'The Assassination of Jesse James by the Coward Robert Ford'
];
{% endhighlight %}

Um den Wert eines Elements zu erhalten benötigt man dessen Position. Diese Position
nennt man Index. Der Index beginnt immer bei `0`. Um einen bestimmten Index abzufragen
benutzt man eckige Klammern.

{% highlight javascript linenos %}
filme[0]; // 'M'
filme[2]; // 'Up'
{% endhighlight %}

### Objekt

Ein Objekt ist eine Variable die Eigenschaften hat. Diese Eigenschaften haben
einen Namen und einen Wert.

{% highlight javascript linenos %}
var kontakt = {
    name: 'Alice',
    nummer: '+43 9 99 99 999'
}
{% endhighlight %}

Um den Wert einer der Eigenschaften zu erhalten benutzt man einen Punkt.

{% highlight javascript linenos %}
kontakt.name; // 'Alice'
kontakt.nummer; // '+43 9 99 99 999'
{% endhighlight %}

Außerdem ist es in JavaScript auch möglich Eigenschaften von Objekten mittels
eckigen Klammern abzufragen.

{% highlight javascript linenos %}
kontakt['name']; // 'Alice'
kontakt['nummer']; // '+43 9 99 99 999'
{% endhighlight %}
