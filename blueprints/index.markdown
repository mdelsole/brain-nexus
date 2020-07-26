---
layout: page
type: section
status: publish
published: true
title: Blueprints
date: '2011-05-08 08:24:33 +0200'
date_gmt: '2011-05-08 08:24:33 +0200'
categories: []
tags: []
---

In the **Brain Architecture** guide we learned the biological properties of every aspect of the brain. In the **Computational Neuroscience** guide we learned the computational properties of every aspect of the brain; the emergent phenomenon created by the sum of the biological properties.

Here in the Blueprints guide, we're going to put it all together. We will take every important aspect of the brain, biological and functional, and use it to make blueprints of how to create a brain.

This will be the last section to be completed. I'll be filling it out as I learn from filling every other section out.


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