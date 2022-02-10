---
layout: default
title: RS_ github page
permalink: index.html
---

# rsunderscore.github.io
gihtub hosted site

- a link to the [blog post]({{post_url 2022-02-07-test-post.md }})
- a link to the [resume](Sunderland5 2021.pdf)
- abs link to [npr](http://npr.org/)

<p>testing liquid in html tags: post url is {{post_url 2022-02-07-test-post.md }} 
and the date for the page is {{page.date}} 
and the author is {{page.author}}
</p>

{{ page.date }} - Written by {{ page.author }}


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
