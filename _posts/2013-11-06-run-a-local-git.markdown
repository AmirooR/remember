---
layout: post
title: "Run a git server locally"
date: 2013-11-06 14:31:15
categories: git local gitbucket
---

# Download gitbucket and run
You should first download the latest version [gitbucket.war][gitbucket].
Then, run the following command:

{%highlight bash %}
java -jar gitbucket.war --port=8888
{%endhighlight}

You could also deploy it on a j2ee server like tomcat7 ( I have not tested it though ).

[gitbucket]: https://github.com/takezoe/gitbucket/releases
