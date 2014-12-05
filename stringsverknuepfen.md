---
title: Strings verknüpfen
toc: 9
---
# {{ page.title }}

Um variable und statische Strings aneinander zu hängen müssen sie verknüpft werden.
Dies kann so aussehen:

{% highlight javascript linenos %}

var name = 'Amy';

anzeigeText = 'Name: ' + name;

alert(anzeigeText);

{% endhighlight %}

Der Inhalt der Variable `name` wird mit dem String `'Name: '` verknüpft und kann
dann angezeigt werden.
