﻿---
layout: page
title: iwware
---
{% for tag in site.tags %}

##### {{ tag[0] }}

{% for post in tag[1] %}

 - [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date_to_string }}</small>

{% endfor %}

{% endfor %}
