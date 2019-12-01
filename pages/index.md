---
layout: page
title: Index
subtitle: Index of all the posts
permalink: /index/
tags: [index]
---

<h2>{{ site.data.samplelist.docs_list_title }}</h2>
<ul>
   {% for item in site.posts %}
      <li><a href="{{ item.url }}">{{ item.title }}</a>{{ item.date | date: "%B %-d, %Y" }}</li>
      page.date
   {% endfor %}
</ul>

