---
layout: default
title: rsunderscore.github.io
permalink: index.html
author: RS_
date: 2022-02-11
description: main portal page
---


Currently attempting to get my bearings and brush-up on web development so that I can make this site more robust.  Hopefully that will also help me with Flask and Django sites, if I find a place to host them in the future.  This page will act as a portal to project documentation, blog posts, and other resources as I find them.  

You can get my history on the [about](about.html) page if that is of interest to you.


## links
- [github main page](http://github.com/rsunderscore)
- [linkedin profile](https://www.linkedin.com/in/robert-sunderland-a072a457/)
- [FAIQ](FAIQ.html) (Frequently Asked Interview Questions)
- [medium.com blog](http://medium.com/@rsunderscore) initial attempts at blog posts - I might mirror some of these blogs on the other site

## Resume
A [pdf version of my resume](Sunderland5 2021.pdf) is available.

## Blog <a id="blog" ></a>
Blog entries are listed below (most recent first).  

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> by {{post.author | default: site.author}} - {{post.date | date: "%Y-%m-%d"}}
    </li>
  {% endfor %}
</ul>

## Projects<a id='projects'></a>

- [Higher Education Scorecard Analysis](highered)
- Spanish NLP
- Job Posting NLP

## to-do
- [x] research sassy css (used by jekyll sites)
	- sassy css is an extension of css which is an interpretted language compile to regular css by the sass executable
		- can be set up to run on a specified file or to 'watch' a directory for changes
	- two file types - both can reside in assets/css for the purpose of jekyll
		- scss - this is the new format and is more css like in syntax
			- statements end with ; and blocks are specified by braces {}
		- sass - this is the older format which is more python-like
			- no semicolon to end statements and blocks are indicated by indentation
	- inheritance
		- can include other files
		- can define mixin tags that can be re-used
	- variables
		- can bet set to single values or whole sections of css
		- set a width once and use it multiple times
	- nesting - allows you to extend the definition for included elements by specifying another tag
		- e.g. &-h1 would be an h1 tag inside the outer element (css version woudl require specifying the entire definition again)
- [x] FAIQ page
- [ ] [Alembic](https://github.com/daviddarnes/alembic) theme?
	- font is called Merriweather on fonts.google.com

the date for the page is {{page.date}} 

Written by {{ page.author }}

test image below

<a title="Tobias Hanf, CC BY-SA 3.0 &lt;https://creativecommons.org/licenses/by-sa/3.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Circuit_Board_(260854457).jpeg">
	<img width="128" alt="Circuit Board (260854457)" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/13/Circuit_Board_%28260854457%29.jpeg/128px-Circuit_Board_%28260854457%29.jpeg">
</a>

HTML unicode entity: &#x1F304;


