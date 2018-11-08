---
layout: post
title:  "Git merge without pain"
date:   2018-11-06 19:54:00 +0300
categories: git rebase commit merge
---
Все мы сталкивались с болью, которая возникает при разрешении конфликтов 
remote и локальной ветки. Кто-то пользуется `git merge`, другие используют
`git rebase`, но такая проблема время от времени все равно возникает и у тех, 
и у других.

Я хочу рассказать о том, что я делаю, чтобы минимизировать время, потраченное
на решение конфликтов.

## **git rebase** preserves names

Сразу обратимся к примерам.

*baz.py*

{% highlight python %}
def f():
    pass
{% endhighlight %}

