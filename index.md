---
layout: page
title: Politely, Up Yours!
tagline: A podcast that dives deep on understanding the world in which we live with thoughtful hosts coming from entirely different perspectives.
---
{% include JB/setup %}

## Latest Episode

{% for post in site.posts limit:1 %}
  [{{ post.title }}]({{ BASE_PATH }}{{ post.url }})
  {{ post.date | date_to_string }}
  <audio src="{{ post.link }}" controls="controls"></audio>
  [Download]({{ post.link }}){:target="_blank"}
{% endfor %}

## Recent Shows

{% for post in site.posts limit:6 offset:1 %}
  [{{ post.title }}]({{ BASE_PATH }}{{ post.url }})
  {{ post.date | date_to_string }}
{% endfor %}
