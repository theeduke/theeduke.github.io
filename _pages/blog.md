---
title: "Blog"
permalink: /blog/
layout: splash
author_profile: true
---
#Blog
#My latest thoughts and insights on software development, backend engineering, and technology trends. Posts are sourced from my Medium blog. 
#{% for post in site.remote_feed.posts limit:5 %}

#[{{ post.title }}]({{ post.url }}){{ post.date | date: "%B %d, %Y" }}{{ post.excerpt | strip_html | truncatewords: 30 }}{% endfor %}
<h1>Blog</h1>
<p>My latest thoughts and insights from Medium:</p>

<ul>
  {% if site.remote_feed.posts %}
    {% for post in site.remote_feed.posts %}
      <li>
        <a href="{{ post.url }}" target="_blank">{{ post.title }}</a>
        <br><small>{{ post.date | date: "%B %d, %Y" }}</small>
        <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      </li>
    {% endfor %}
  {% else %}
    <li>No posts found or feed failed to load.</li>
  {% endif %}
</ul>


testing: <pre>{{ site.remote_feed | inspect }}</pre>


<ul>
  {% for post in site.remote_feed.posts limit:5 %}
    <li>
      <a href="{{ post.url }}" target="_blank">{{ post.title }}</a><br>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    </li>
  {% endfor %}
</ul>


