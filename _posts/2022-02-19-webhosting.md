---
layout: post
title: "Python Web Hosting"
tags: python web flask django
author: RS_
---

# Python web hosting
by {{page.author}}
{{ page.date }}


One of my goals was to create a web site to facilitate blog posts, because medium.com was not syntax highlighting the code.  Syntax highlights for code on implicit on the github.io site.  One of my other web hosting goals is to set up interactive web applications.  But since github.io is only for static sites, that isn't an option.  My machine learning book has a chapter on deploying machine learning models using flask, and leveraged pythonanywhere.com as the hosting solution.  Pythonanywhere is free for basic implementations but I wanted to do some research and gather other options and compile the information here so that I could refer back when the time comes.

###Starting with 'best-of' lists:
[12 best python hosting services](https://www.hostingadvice.com/how-to/best-python-hosting/) - warns agains free hosting – 'python apps won't run optimally'... security, no plugins
	- siteground - $3.99/mo – SSL, business email
	- bluehost – $2.95/mo – website builder/templates, SSL, $7.99/mo, free domain
	- hostinger - $1.39/mo – google cloud ($10), site builder, SSH/SSL
	- hostgator - $2.64/mo – SSL, email, domain
	- iPage - $1.99/mo – marketing, ecommerce
	- inMotionHosting - $2.79/mo – SSD, SSL, 
	- cloudways - $10/mo - cloud (multiple providers)
	- hostwinds - $4.99/mo

[8 best hosting platforms](https://geekflare.com/python-hosting-platform/) - python history (not on topic) 
	- platforms.sh – template libraries – git based workflow
	- inset: Kamatera - $4/mo – django-only hosting – no further information
	- a2 hosting - $2.99/mo – speed/uptime
	- chemicloud - $6.95/mo – SSD/speed - PHP
	- pythonanywhere – django/flask – numpy/scipy, pycrypto, bs4 (Amazon EC2 host)
	- fastcomet – fast/SSD - tutorials
	- heroku – github, metrics, django/flask
	- nodechef – SSD, github, MongoDB
	- google cloud

[best free django hosting](https://freedjango.com/free-django-hosting/) - credibility of this site is suspect based on some of the other content – content is simlar to other sites suggesting they may have just scraped someone else article.  Broken english suggests a poor translation.  Also odd that the intent is 'free' hosting but they list mostly fee sites.  
	- A2 - $2.99/mo
	- BlueHost - $3.94/mo
	- YouStable – requires custom domain – no cost for this offering listed
	- Heroku – free or $6.98/mo
	- PythonAnywhere – free or $4.99/mo

[6 best python hosting services](https://www.websiteplanet.com/blog/best-python-hosting-services/)
	- interserver - $6/mo – webuzo(replaced CLI?)
	- kamatera - $4/mo – SSD, hourly
	- hostinger (mentioned as best in summary but no detail)
	- a2 – no django (only flask)
	- siteground – only Python2?
	- Liquidweb - $15/mo - hands-off
	- hostpapa - $20/mo - 


## Further exploration

### [pythonanywhere](https://www.pythonanywhere.com/)
	- 512 MB disk (free tier)
	- deploy from github
	- web based programming (mobile)
	- python 3.8
	- Flask and Django support

### Heroku

### a2

### bluehost

### [google cloud hosting](https://cloud.google.com/python/)
	- using [google cloud for python](https://cloud.google.com/python/docs/getting-started)
	- [pricing calculator](https://cloud.google.com/products/calculator)
	- 'always free' tier of service
	- pieces for python app: [app engine](https://cloud.google.com/appengine/docs), cloud storage, firestore (noSQL document DB), operations suite
	-  Free trial (90 days)
	- [ToS](https://cloud.google.com/terms/?_ga=2.150684854.1669371226.1645306337-140689797.1645306337) - “Customer owns all Intellectual Property Rights in Customer Data and Customer Applications, and Google owns all Intellectual Property Rights in the Services and Software. ” -  “Google will only access or use Customer Data to provide the Services and TSS to Customer or as otherwise instructed by Customer and will not use it for any other Google products, services, or advertising. ”
	- [supplemental trial terms](https://cloud.google.com/terms/free-trial/?_ga=2.150684854.1669371226.1645306337-140689797.1645306337)  0- 8 cores - 
	- [terms](https://console.cloud.google.com/terms) for other services – look up ones that apply to you


## Glossary
VPS – [virtual private server](https://en.wikipedia.org/wiki/Virtual_private_server) – usu single VM on shared host – user has root access; I expect this means you would need to install/maintain your own web server instance in addition to all the python packages and frameworks need for the app itself
VDS – virtual dedicates server
