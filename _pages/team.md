---
title: "Roychoudhuri Lab - Team"
layout: gridlay
excerpt: "Roychoudhuri Lab: Group members"
sitemap: false
permalink: /team/
---
<h3 style="margin-top:0px">Group Members</h3> 


 **We are looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**



{% assign number_printed = 0 %}
{% assign members_sorted = site.members | sort: 'tier' %}
{% for member in members_sorted %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}{{ member.url }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/member_pic/{{ member.picture }}" class="img-responsive" width="25%" style="float: left" /></a>
  <h4> <a style="text-decorations:none; color:inherit;" href="{{ site.url }}{{ site.baseurl }}{{ member.url }}">{{ member.fullname }}</a></h4>
  {{ member.position }}<br>
  email: {{ member.email }}<br>
  <i>>> <a style="text-decorations:none; " href="{{ site.url }}{{ site.baseurl }}{{ member.url }}">More information</a></i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br />
<h3>Collaborators</h3>
We benefit from extensive interactions with reseachers in many different groups, including the following:
{% for item in site.data.collaborations %}

{% if item.link %}<b><a href="{{ item.link }}">{% endif %}{{ item.title }}{% if item.link %}</a></b>
{% endif %}
{% endfor %}

<br />
<h3>Facilities</h3>
The laboratory has access to the world-class research facilities of the University of Cambridge School of the Biological Sciences and the Department of Pathology, which provide state-of-the-art equipment, technical advice, and training. The facilities have an emphasis on quality and consistency and are vital in helping us deliver world-class research. Read more about [Research Facilities at the School of the Biological Sciences](https://www.bio.cam.ac.uk/facilities), and [Research Facilities at the Department of Pathology](https://www.path.cam.ac.uk/research/facilities). The following are facilities we make frequent use of:

{% for item in site.data.facilities %}
{% if item.link %}<b><a href="{{ item.link }}">{% endif %}{{ item.title }}{% if item.link %}</a>
</b>{% endif %}
{% endfor %}

<br />