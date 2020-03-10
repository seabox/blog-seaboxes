---
layout: page
title: Index
permalink: /index/
color: rgb(0, 160, 130)
tags: [index]
---

   {% for item in site.posts %}
* <a href="{{ item.url }}">{{ item.title }}</a> {{ item.date | date: "%-d %B %Y" }}
   {% endfor %}

