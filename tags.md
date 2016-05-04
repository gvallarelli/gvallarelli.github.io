---
layout: post
title: Tags
---
<!-- categories --> 
{% assign sortedtags = site.tags | sort %}
{% for tag in sortedtags %}
<div class="box">
  <a name="{{ tag | first | cgi_escape }}"></a>
  <h1>{{ tag | first }}</h1>
  <ul class="postList"> 
  {% for posts in tag %}
    {% for post in posts %}
      {% if post.title %}
        <li>
          {{ post.date | date: "%Y/%m/%d" }}: <a href="{{ post.url }}">{{post.title}}</a>
        </li>
      {% endif %}
    {% endfor %}
  {% endfor %}
  </ul>
</div>        
{% endfor %}
