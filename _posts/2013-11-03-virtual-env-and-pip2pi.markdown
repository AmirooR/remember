---
layout: post
title: "Using python virtualenv and pip2pi for local packages"
date: 2013-11-03
categories: python virtualenv pip2pi
---
## Install pip and set virtualenv
{% highlight bash %}
sudo apt-get install python-pip 
sudo pip install virtualenv
cd ~/workdir
virtualenv venv
. venv/bin/activate
{%endhighlight%}

## Downloading Packages
{% highlight bash %}
pip2pi example.com:/var/www/packages/ -r requirements.txt
#=> installs packages in requirement.txt
#=> remove example.com: for downloading locally
{% endhighlight %}

## Installing New Package Index
{% highlight bash %}
pip install --index-url=http://example.com/packages/simple/ -r requirements.txt
{% endhighlight %}


