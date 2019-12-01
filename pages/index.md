---
layout: page
title: Index
subtitle: Index of all the posts
permalink: /index/
tags: [index]
---

## {{ site.data.samplelist.docs_list_title }}

   {% for item in site.posts %}
* <a href="{{ item.url }}">{{ item.title }}</a> {{ item.date | date: "%B %-d, %Y" }}
   {% endfor %}

