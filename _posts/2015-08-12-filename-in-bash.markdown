---
layout: post
title: "Handling filename and extensions in bash"
date: 2015-08-12
categories: bash filename
---
Get file without path

{% highlight bash %}
filename=$(basename "$fullfile")
extension="${filename##*.}"
filename="${filename%.*}"
{%endhighlight%}

You can focus on the last '/' of the path instead of '.' which should work even if you have unpredictable file extension:

{% highlight bash %}
filename="${fullfile##*/}"
{% endhighlight %}


