---
title: Blog
permalink: /blog/
layout: splash
---
Blog
My latest thoughts and insights on software development, backend engineering, and technology trends. Posts are sourced from my Medium blog. 
{% for post in site.remote_feed.posts limit:5 %}

[{{ post.title }}]({{ post.url }}){{ post.date | date: "%B %d, %Y" }}{{ post.excerpt | strip_html | truncatewords: 30 }}{% endfor %}

