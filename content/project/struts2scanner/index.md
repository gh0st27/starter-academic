---
title: Struts2Scanner
date: 2021-02-10T14:34:54.186Z
summary: "Struts2Scanner is a python based tool to detect struts2 vulnerabilities on the website."
draft: false
featured: true
tags:
  - Python
  - Scanner
  - Struts2
categories:
  - Python
external_link: ""
links:
- icon: github
  icon_pack: fab
  name: Follow
  url: https://github.com/gh0st27/Struts2Scanner
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
---
Apache Struts is a free, open-source framework for creating elegant, modern Java web applications. It has its share of critical vulnerabilities, with one of its features, OGNL – Object-Graph Navigation Language, being at the core of many of them.

Struts2Scanner is a vulnerability scanner to find out if a target endpoint is vulnerable to struts2 vulnerabilities. Currently it checks against following vulnerabilities.

* cve-2020-17530
* cve-2019-0230
* cve-2018-11776
* cve-2017-5638
* cve-2017-9791

## How to use
```
root@kali:/home/Struts2Scanner# python3 Struts2Scanner.py -h
usage: Struts2Scanner.py [options] --url "http://www.site.com/vuln.php?id=1"

optional arguments:
  -h, --help         show this help message and exit
  -u URL, --url URL  Target URL (e.g."http://www.site.com/vuln.php?id=1&fname=test&lname=tester")
  --data DATA        Data string to be sent through POST (e.g. "id=1&fname=test&lname=tester")
  --cookies COOKIES  HTTP cookies (eg. "jsessionid=1234")
  --proxy PROXY      Use a proxy to connect to the target URL

```
![Capture](/Capture.PNG)
## Requirements
* Python3
* Check requirements.txt file

## Installation Steps
```pip3 install -r requirements.txt```

