---
layout: default
title: rsunderscore.github.io
permalink: index.html
author: RS_
date: 2022-02-11
description: ''
---


Currently attempting to get my bearings and brush-up on web development so that I can make this site more robust.  Hopefully that will also help me with Flask and Django sites, if I find a place to host them in the future.  This page will act as a portal to project documentation, blog posts, and other resources as I find them.  

You can get my history on the [about](about.html) page if that is of interest to you. Or check out the [pdf version of my resume](Sunderland5 2021.pdf).


## links
- [github main page](http://github.com/rsunderscore)
- [linkedin profile](https://www.linkedin.com/in/robert-sunderland-a072a457/)
- [FAIQ](FAIQ.html) (Frequently Asked Interview Questions)
- [medium.com blog](http://medium.com/@rsunderscore) initial attempts at blog posts - I might mirror some of these blogs on the other site

## Recent Blog Entries <a id="blog" ></a>
These are the 5 most recent; you can also view the [full list](blog.html).

<ul>
{% assign count = 0 %}
  {% for post in site.posts %}
  {% assign count = count | plus:1 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>  -- <span style="text-align: right;"> {{post.date | date: "%Y-%m-%d"}} </span>
    </li>
	{% if count == 5 %}{% break %}
	{% endif %}
  {% endfor %}
</ul>
## Projects<a id='projects'></a>

- [Higher Education Scorecard Analysis](highered)
- Spanish NLP
- Job Posting NLP




{% comment %}
the date for the page is {{page.date}} 
Written by {{ page.author }} 
{% endcomment %}

test image below

<a title="Tobias Hanf, CC BY-SA 3.0 &lt;https://creativecommons.org/licenses/by-sa/3.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Circuit_Board_(260854457).jpeg">
	<img width="128" alt="Circuit Board (260854457)" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/13/Circuit_Board_%28260854457%29.jpeg/128px-Circuit_Board_%28260854457%29.jpeg">
</a>

HTML unicode entity: &#x1F304;


