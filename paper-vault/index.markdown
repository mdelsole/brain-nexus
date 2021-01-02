---
layout: page
type: section
status: publish
published: true
title: Paper Vault
date: '2011-05-08 08:24:33 +0200'
date_gmt: '2011-05-08 08:24:33 +0200'
categories: []
tags: []
---

When you arrive at the higher-level functions of the brain, the information you'll be able to find from textbooks wears thin. To find the information you're looking for, you have to dive into the world of research papers.

There are thousands of reasearch papers out there that contain valuable information. Unfortunately, they are written in non-layman's terms, and require a great deal of effort to read thoroughly. 

While one can certainly read these papers, it is a completely different matter to be able to efficiently extract information from them. The time investment for the inexperienced is considerably more than that of a textbook chapter, which has already extracted the information of many papers for you. 

I read many papers in my quest to design AGI, and I've found the best way for me to get the most out of them is to take detailed notes on their content. Consider this section a **paper summarizer**; I will take the useful information from papers, mixed in with my notes and ideas, and post them here.



{% assign sorted_pages = site.pages | sort:"order" %}
{% for p in sorted_pages %}
   {% assign splt = p.url | split: page.url %}
   {% if splt.size == 2 and splt[0] == '' %}
      {% assign slash = splt[1] | split: '/' %}
{% if slash.size == 1 %}      
- <a class="page-link" href="{{p.url | prepend: site.baseurl}}">{{p.title}}</a>
{% else %}
   - <a class="page-link" href="{{p.url | prepend: site.baseurl}}">{{p.title}}</a>
{% endif %}
   {% endif %}
{% endfor %}