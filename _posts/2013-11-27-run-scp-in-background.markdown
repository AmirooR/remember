---
layout: post
title: "Run SCP in background"
date: 2013-11-27 17:53:15
categories: shell scp background
---

* Run scp as usual:

{% highlight bash %}
scp user@server:/home/gholi/gholi.txt .
{%endhighlight %}

Then type password.

* Background the scp: 

{% highlight bash %}
Ctrl+Z
{%endhighlight %}

* Continue it: 

{% highlight bash %}
bg
{%endhighlight %}

* Disown the background process:

{% highlight bash %}
disown
{%endhighlight %}


Now you can exit while the program is still running.

check this [stackexchange][stack] page for more info.

[stack]: http://unix.stackexchange.com/questions/65116/does-a-scp-transfer-close-when-i-close-the-shell

