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

### Objekt

Ein Objekt ist eine Variable die Eigenschaften hat. Diese Eigenschaften haben einen Namen und einen Wert.

{% highlight javascript linenos %}
var kontakt = {
    name: 'Alice',
    nummer: '+43 9 99 99 999'
}
{% endhighlight %}

