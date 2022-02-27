---
layout: post
title:  "Possible Project"
categories:
tags: minipost project idea
---

- document similarity using gensim
- examine job postings and compare simlarity to each other
- maybe do some usupervised classification or clustering
- use tf/idf or cosine similarity
- word2vec or doc2vec might be other options
- numpy or Spacy for the NLP parts?
- compare similarity to resume
- parse skill requirements out of a job posting

It would be nice to pull a lot of job postings to use as the corpus for the model. Indeed has some sparse API documentation. Most of their documentation is focused on people creating web-apps where they would allow a visiting usering to authenticate to their Indeed account using Oauth tokens. In my case, I just want to pull a lot of data for myself, not act on behalf of other users. (I ran into this same problem when I tried to research API calls for LinkedIn.) There was a nice blog on medium.com that talks about pulling job search results from Indeed API, and mentions that a publisher ID is required. The publisher documentation is even more sparse and the difficulty in finding it from the indeed main site made me suspicious. In the end I just used very generic credentials so we'll see if that gets a successful review.


{% comment %} tags: {{ page.tags | join: ", " | prepend: "\#"}} {% endcomment %}

{% for tag in page.tags %} #{{tag}}, {%endfor%}
