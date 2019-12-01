---
layout: page
title: Index
permalink: /index/
color: rgb(10,70,10)
tags: [index]
---

   {% for item in site.posts %}
* <a href="{{ item.url }}">{{ item.title }}</a> {{ item.date | date: "%B %-d, %Y" }}
   {% endfor %}

