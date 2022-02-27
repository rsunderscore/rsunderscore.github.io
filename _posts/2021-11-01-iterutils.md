---
layout: post
title:  "iterutils and more"
categories:
tags: minipost
---
Spent some time reading through the documentation for more-iterutils, which solves all problems everywhere, but mostly the one I mentioned last week. Chunked is the method they use to split a list into sublists and it does exactly what I wanted. more-iterutils is not part of the standard library, unlike iterutils; so it's not quite as readily available. It has a plethora of other useful tools that certainly make it worth it. 'Convolve' was one that stumped me for a while. I am familiar with converolutional neural networks and how they process images, but the linear convolution was foreign to me. After consulting several math-oriented sites I was able to reproduce the output in a spreadsheet which gave me some joy.

Not very happy with progress on the rawg dataset. Some of the fields I wanted aren't there and I'm not confident that the use case I've selected is really machine learning or just an improved version of search. I might have to pivot to a new use case. Perhaps unsupervised classification. Alternatively, I could augment the data with other data sources.