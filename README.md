---
layout: default
title: RS_ github page
permalink: index.html
author: RS_
date: 2022-02-11
description: main rs_ github page
---

# main page for RS_ github
Currently attempting to get my bearings and brush-up on web development so that I can make this site more robust.  Hopefully that will also help me with Flask and Django sites, if I find a place to host them in the future.  This page will act as a portal to project documentation, blog posts, and other resources as I find them.  

You can get my history on the [about](about.html) page if that is of interest to you.

sit var: {{ site.email }}

## links
- github main page
- linkedin profile
- FAIQ (Frequently Asked Interview Questions)
	- talk about a time you were successful, what was the project and how did it improve things?
	- talk about a time when you were not successful, what were the repercussions and how did you deal with them?
	- how do you deal with conflict in the workplace?
	- what is the importance of diversity?
	- how do you handle situations where you have to follow a decision you don't agree with?

## Resume
A [pdf version of my resume](Sunderland5 2021.pdf) is available.

## Blog
Blog entries are listed below (most recent first).  

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> by {{post.author | default: site.author}} - {{post.date | date: "%Y-%m-%d"}}
    </li>
  {% endfor %}
</ul>

## Projects

- [Higher Education Scorecard Analysis](highered)
- Spanish NLP
- Job Posting NLP

## to-do
- [ ] research sassy css (used by jekyll sites)
- [ ] FAIQ page

the date for the page is {{page.date}} 

Written by {{ page.author }}

test image below

<a title="Tobias Hanf, CC BY-SA 3.0 &lt;https://creativecommons.org/licenses/by-sa/3.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Circuit_Board_(260854457).jpeg">
	<img width="128" alt="Circuit Board (260854457)" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/13/Circuit_Board_%28260854457%29.jpeg/128px-Circuit_Board_%28260854457%29.jpeg">
</a>

HTML unicode entity: &#x1F304;


