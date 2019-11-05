---
title: "RT2 Lab - Team"
layout: gridlay
excerpt: "RT2 Lab: Team members"
sitemap: false
permalink: /team/
---

## Group Members

{% for team in site.data.team_members %}
<h3>{{team.display_name}}</h3>

<div class="card-group">
{% for member in team.members %}
<div class="card mb-3" style="max-width: 400px;">
<div class="row no-gutters">
<div class="col-md-4">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="card-img img-responsive" />
</div>
<div class="col-md-8">
<div class="card-body">
<h5 class="card-title">{{ member.name }}</h5>
<p class="card-text">{{ member.info }}</p>
<ul>
{% for education in member.education %}
<li>{{education}}</li>
{% endfor %}
</ul>
<p class="card-text"><small class="text-muted">Contact: <{{member.email}}></small></p>
</div>
</div>
</div>
</div>
{% endfor %}
</div>

{% endfor %}
