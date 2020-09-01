---
layout: page
permalink: /history
title: Categories
---



{% for post in site.categories.history %}
 
<ul id="archive">
<li class="archiveposturl"><span><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></span><br/>

<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:left; padding-right: .5em">{{ post.source}}</strong> 
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">{{ post.date | date: '%d %b %Y' }}</strong> 

</li>
</ul>

{% endfor %}
