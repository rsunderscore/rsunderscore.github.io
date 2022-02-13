---
layout: default
title: RS_ github page
permalink: index.html
author: fred
date: 2022-02-11
---

# rsunderscore.github.io
gihtub hosted site

- a link to the [blog post]({%post_url 2022-02-07-test-post %})
- a link to the [resume](Sunderland5 2021.pdf)
- abs link to [npr](http://npr.org/)

<p>testing liquid in html tags: 
the date for the page is {{page.date}} 

and the author is {{page.author}}
</p>

{{ page.date }} - Written by {{ page.author }}

test image below
<a title="Tobias Hanf, CC BY-SA 3.0 &lt;https://creativecommons.org/licenses/by-sa/3.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Circuit_Board_(260854457).jpeg">
	<img width="128" alt="Circuit Board (260854457)" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/13/Circuit_Board_%28260854457%29.jpeg/128px-Circuit_Board_%28260854457%29.jpeg">
</a>

&#x1F304;


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
