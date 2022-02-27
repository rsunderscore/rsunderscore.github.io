---
layout: post
title:  "quick useful utility"
categories:
tags: minipost
---
useful utility for splitting up an iterable into smaller lists - there are many way to do this but I settled on this one because it doesn't use any additional modules
```python
def splititer(aniter, maxlen):
    cuts = [x for x in range(0, len(aniter),maxlen)] + [len(aniter)]
    newlist = [aniter[cuts[i]:cuts[i+1]] for i in range(len(cuts)-1)]
    return newlist
```