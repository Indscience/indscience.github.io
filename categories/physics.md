---
layout: page
permalink: /categories/history
title: Categories
---



{% for post in site.categories.physics %}
 
<ul id="archive">
<li class="archiveposturl"><span><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></span><br/>
<span class = "postlower">

<!-- <strong>Author:</strong> {{post.author}} -->
<strong>Category:</strong>  {% if post.categories %}
 
  {% for cat in post.categories %}
  <a href="/categories/#{{ cat }}" title="{{ cat }}">{{ cat }}</a>&nbsp;
  {% endfor %}

{% endif %} <!-- {{ post.categories | first }} -->
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">{{ post.date | date: '%d %b %Y' }}</strong> 
</span> 

</li>

</ul>

{% endfor %}
