---
layout: post
title: "Python Web Hosting"
tags: python web flask django
author: RS_
---

One of my goals was to create a web site to facilitate blog posts, because medium.com was not syntax highlighting the code.  Syntax highlights for code on implicit on the github.io site.  One of my other web hosting goals is to set up interactive web applications.  But since github.io is only for static sites, that isn't an option.  My machine learning book has a chapter on deploying machine learning models using flask, and leveraged pythonanywhere.com as the hosting solution.  Pythonanywhere is free for basic implementations but I wanted to do some research and gather other options and compile the information here so that I could refer back when the time comes.

A few of the hosts use older python versions (e.g. a2 and bluehost): because it comes with their OS deploy or perhaps by choice. Most Linux distros shipped with python 2.7 even though Python ended their support in 2020.  Presumably this is because you don't need the latest features to do basic OS scripting and that is largely what they need to support.  For web development puposes this means we might need to upgrade/install a newer version, which might require a higher tier of hosting or VPS.  If we also have to support our custom installs, rather than focus on support for the web app; this becomes very unattractive.

I perused a few 'best-of' articles to look for services that were well-liked.  Most of these sites are unfamiliar to me, and not backed by major publications; so I did my own research for the companies listed to verify the features and pricing.  It was difficult to get similar data points from each site, even moreso for python hosting details as this was not the primary offering for most of the companies.  Based on this I assume that these companies drive to get your static web hosting account and then leverage whatever app platform is available when the time comes.   Web apps are likely to be for companies that have the additional resources to adapt the offering supported or buy a separate service.

### desired features
- python 3.8
- apache 2.0
- SSL
- domain
- support for both flask and django
- deploy from github
- DB offering
- simplicity

### Starting with 'best-of' lists:


[12 best python hosting services](https://www.hostingadvice.com/how-to/best-python-hosting/) - warns agains free hosting ??? 'python apps won't run optimally'... security, no plugins
- siteground - $3.99/mo ??? SSL, business email
- bluehost ??? $2.95/mo ??? website builder/templates, SSL, $7.99/mo, free domain
- hostinger - $1.39/mo ??? google cloud ($10), site builder, SSH/SSL
- hostgator - $2.64/mo ??? SSL, email, domain
- iPage - $1.99/mo ??? marketing, ecommerce
- inMotionHosting - $2.79/mo ??? SSD, SSL, 
- cloudways - $10/mo - cloud (multiple providers)
- hostwinds - $4.99/mo

[8 best hosting platforms](https://geekflare.com/python-hosting-platform/) - python history (not on topic) 
- platforms.sh ??? template libraries ??? git based workflow
- inset: Kamatera - $4/mo ??? django-only hosting ??? no further information
- a2 hosting - $2.99/mo ??? speed/uptime
- chemicloud - $6.95/mo ??? SSD/speed - PHP
- pythonanywhere ??? django/flask ??? numpy/scipy, pycrypto, bs4 (Amazon EC2 host)
- fastcomet ??? fast/SSD - tutorials
- heroku ??? github, metrics, django/flask
- nodechef ??? SSD, github, MongoDB
- google cloud

[best free django hosting](https://freedjango.com/free-django-hosting/) - credibility of this site is suspect based on some of the other content ??? content is simlar to other sites suggesting they may have just scraped someone else article.  Broken english suggests a poor translation.  Also odd that the intent is 'free' hosting but they list mostly fee sites.  
- A2 - $2.99/mo
- BlueHost - $3.94/mo
- YouStable ??? requires custom domain ??? no cost for this offering listed
- Heroku ??? free or $6.98/mo
- PythonAnywhere ??? free or $4.99/mo

[6 best python hosting services](https://www.websiteplanet.com/blog/best-python-hosting-services/)
- interserver - $6/mo ??? webuzo(replaced CLI?)
- kamatera - $4/mo ??? SSD, hourly
- hostinger (mentioned as best in summary but no detail)
- a2 ??? no django (only flask)?
- siteground ??? only Python2?
- Liquidweb - $15/mo - hands-off
- hostpapa - $20/mo - 


## Further exploration

### [pythonanywhere](https://www.pythonanywhere.com/)
- free tier - username.pythonanywhere.com
	- 512 MB disk (free tier)
	- no Jupyter notebook support
	- one web app
	- 1 web 'worker'
- $5/mo
	- IDE in browser
	- one web app
	- 100k hits/day
	- jupyter support
	- 1 GB disk
	- ssh access
	- 2 web 'workers'
- [databases](https://help.pythonanywhere.com/pages/KindsOfDatabases): mySQL, sqlite or postgres(paid)
	- can connect to databases elsewhere (paid) e.g. [mLab](https://mlab.com/plans/pricing/#plan-type=sandbox&provider=azure) (Mongo) which has 512MB for free or $15/GB
- deploy from github
- web based programming (mobile)
- python 3.8
- Flask and Django support


### [Heroku](https://www.heroku.com/python) ([dev docs](https://devcenter.heroku.com/articles/getting-started-with-python))
- Postgres sql
- owned by salesforce
- Flask or Django
- Free 
        - 1 dyno
	- Sleeps when inactive 30 mins
        - 10k rows db
        - 2 process types
- $7/mo tier "Hobby"
	- Ssl
	- metrics
	- no sleep
	- 10 process types
- next tier up is $25/mo
- Heroku CLI
- GitHub integration
        - deploy to heroku as remote (instead of origin)

### [a2](https://www.a2hosting.com/python-hosting) - site is difficult to navigate and marketing is directed at wordpres
- Django or flask
- MySQL
- 100gb storage
- Python version? Header says 3.2. 3.4 shown in other sections.  In admin guide for python version selection 3.7. compile from source example for 3.8, also mentioned in the article about setting python venv with a script. 
- ssl
- versions list: PHP 5.6, 7.1, 7.2, 7.3, 7.4 or 8.0 (Choose Your Version); MySQL 5.6/MariaDB; PostgreSQL 9.6; <span style="color:red; font-weight: bold;">Python 3.4</span>     PERL 5.10; Apache 2.4; Node.js 12; FTP / SFTP; Free SSH Access; SSL & Free SSL
- Website builder

### [bluehost](https://www.bluehost.com/help/article/python-installation)
"uses the default python version that comes with [CentOS](https://www.centos.org/) by default" - currently av v7-2009 (assuming it is not Python3 given the number of articles on how to install) - not sure if lower tier offerings support a python installation (VPS start at $19/mo).
- $2.75/mo (promotion) $10/mo regular
	- 1 website
	- 50GB storage
	- free domain
	- SSL
	- CDN
- $5/mo promotion ($15/mo regular)
	- unlimited websites

### [google cloud hosting](https://cloud.google.com/python/)
- using [google cloud for python](https://cloud.google.com/python/docs/getting-started)
- [pricing calculator](https://cloud.google.com/products/calculator)
- 'always free' tier of service
- pieces for python app: [app engine](https://cloud.google.com/appengine/docs), cloud storage, firestore (noSQL document DB), operations suite
-  Free trial (90 days)
- [ToS](https://cloud.google.com/terms/?_ga=2.150684854.1669371226.1645306337-140689797.1645306337) - ???Customer owns all Intellectual Property Rights in Customer Data and Customer Applications, and Google owns all Intellectual Property Rights in the Services and Software. ??? -  ???Google will only access or use Customer Data to provide the Services and TSS to Customer or as otherwise instructed by Customer and will not use it for any other Google products, services, or advertising. ???
- [supplemental trial terms](https://cloud.google.com/terms/free-trial/?_ga=2.150684854.1669371226.1645306337-140689797.1645306337)  0- 8 cores - 
- [terms](https://console.cloud.google.com/terms) for other services ??? look up ones that apply to you


## Glossary
VPS ??? [virtual private server](https://en.wikipedia.org/wiki/Virtual_private_server) ??? usu single VM on shared host ??? user has root access; I expect this means you would need to install/maintain your own web server instance in addition to all the python packages and frameworks need for the app itself
VDS ??? virtual dedicates server

CDN - [content delivery network](https://en.wikipedia.org/wiki/Content_delivery_network) geographically distributed proxy servesr to increase performance, typically hosted in ISP datacenter
