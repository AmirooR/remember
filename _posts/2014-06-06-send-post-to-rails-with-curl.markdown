---
layout: post
title: "Send a POST request to rails application with curl"
date: 2014-06-06 22:53:24
categories: rails POST curl
---

* Note that we should set content-type to json

* Example:

{% highlight bash %}
curl -X POST -H "Content-Type: application/json" -d \
'{"player": {"name": "test","room_id": 0,"skin_id": 1,"head_id": 2,"torso_id": 3 \
,"legs_id": 4,"x_position": 5,"y_position": 6,"direction": 7,"action": "","gender": "f"}}'\
localhost:3000/players.json
#==> to use the new environment
{%endhighlight %}

check this [stackoverflow][stack] page for more info.

[stack]: http://stackoverflow.com/questions/18690196/how-should-i-format-a-json-post-request-to-my-rails-app
