---
title: "RT2 Lab - Publications"
layout: gridlay
excerpt: "RT2 Lab -- Publications."
sitemap: false
permalink: /publications/
---


## Publications

{% for publi in site.data.publist %}

  <a href="{{ publi.link.url }}">{{ publi.title }}</a><br/>
  <em>{{ publi.authors }}</em><br/>
  <em>{{ publi.journal }}, {{ publi.year }}</em><br/>

{% endfor %}
