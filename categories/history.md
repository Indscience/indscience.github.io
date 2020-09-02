---
layout: page
permalink: /history
title: Categories
---




<ul id="archive">
{% for post in site.categories.history %}
 

<li class="archiveposturl"><span><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></span><br/>

<span class = "postlower">

<!--<strong>Author:</strong> {{post.author}} -->
<strong>source:</strong>  {% if post.source %}
 
  {% for source in post.source %}
  <a href="/source" title="{{ source }}">{{ source }}</a>&nbsp;
  {% endfor %}

{% endif %} 
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">{{ post.date | date: '%d %b %Y' }}</strong> 
</span> 


</li> 

</ul>

{% endfor %}



