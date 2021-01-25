---
title: Stored XSS on Search Engine
subtitle: Stored cross-site scripting (also known as second-order or persistent
  XSS) arises when an application receives data from an untrusted source and
  includes that data within its later HTTP responses in an unsafe way.
date: 2021-01-25T15:41:33.722Z
draft: false
featured: true
authors:
  - admin
tags:
  - BugBounty
  - XSS
  - YesWeHack
image:
  filename: eab580a5286ee9b20e30389342f18861-xss1.png
  focal_point: Smart
  preview_only: false
---
## **Overview**

Stored XSS vulnerability was found on Qwant search engine on February 2020 and was fixed in few hours after the triage

### Proof of Concept

1. Create a blog or website with XSS payload as a title name. I created account on [www.prezi.com](www.prezi.com) & add the blog with title as XSS payload.

![](4aa9535b461a763203c1f761ad98385c-xss2.png)

2. Wait for few days to get your website crawl by the search engine crawler. It took 8 days to crawl & list the website on Qwant search engine crawler.
3. Search the website name.  As you can see XSS payload is executed on the browser.

![](eab580a5286ee9b20e30389342f18861-xss1.png)