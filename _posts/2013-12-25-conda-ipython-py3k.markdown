---
layout: post
title: "Conda configuration with python3 and ipython, etc"
date: 2013-12-25 20:53:24
categories: conda python3 ipython
---

* Create a new environment:

{% highlight bash %}
conda create -n py3k python=3 matplotlib pip ipython pyzmq jinja2 numpy tornado
activate py3k #==> to use the new environment
{%endhighlight %}

* Install new packages to the environment:

{% highlight bash %}
conda install -n py3k pkg
{%endhighlight%}

* Compiling some packages by MS-Visual Studio 2010 requires:

{% highlight bash %}
SET VS90COMNTOOLS=%VS100COMNTOOLS%
{%endhighlight %}


