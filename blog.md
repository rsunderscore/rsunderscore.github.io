---
layout: default
title: Blog 
author: RS_
date: 2022-02-11
description: entries from me
---

## Blog <a id="blog" ></a>
Blog entries are listed below (most recent first).  

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>  -- <span style="text-align: right;"> {{post.date | date: "%Y-%m-%d"}} </span>
    </li>
  {% endfor %}
</ul>
