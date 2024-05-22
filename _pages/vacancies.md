---
title: "Roychoudhuri Lab - Vacancies"
layout: homelay
excerpt: "Openings"
sitemap: false
permalink: /vacancies
---

<h3 style="margin-top:0px">Joining the lab</h3> 

We are looking for new group members with passion, talent, and grit! You will have the chance to work on grand challenges in the field immune regulation and tumour immunity. You will be responsible for driving your research, identifying the most important questions, designing and performing experiments and publishing findings.

Several Postdoc and PhD positions are available over the next few months - please email me with expressions of interest, including a CV. 

#### Applications for Postdoctoral Fellowships 
We are happy to support the most talented postdoctoral researchers to apply for fellowships in the group. Please contact me if you'd like to discuss this route to joining the laboratory.  Please send me an [email](mailto:rr257@cam.ac.uk) stating briefly why you are interested in joining the group and attaching a CV.

#### PhD studentships in the laboratory
I am happy to consider and support applications for PhD studentships. Should funded studentships be available in the laboratory, they will be advertised on the following website:

[Roychoudhuri lab PhD Studentships](https://www.findaphd.com/phds/?Keywords=roychoudhuri)

#### Master's and Bachelor's internships
If you are looking for a Masters project in the laboratory, contact me by email with a copy of your CV, a start and end date of the internship, and a brief statement of why you'd be interested in joining the laboratory.

<div style="width:100%; display: inline-block; float:none; vertical-align: top; clear: both;">
 {% include carousel.html %}
 </div>

<h3 style="margin-top:0px">Group Members</h3> 

 **You'd be joining a friendly, motivated, and highly collaborative team in a leading research environment in the heart of Cambridge**
 
{% assign members_sorted = site.members | sort: 'tier' %}
{% for member in members_sorted %}

  <b><a style="" href="{{ site.url }}{{ site.baseurl }}{{ member.url }}">{{ member.fullname }}</a></b>, {{ member.position }}. Email: {{ member.email }}.<br /><i>» <a style="text-decorations:none; " href="{{ site.url }}{{ site.baseurl }}{{ member.url }}">More information</a></i><br>

{% endfor %}


<h3>Collaborators</h3>
We benefit from extensive interactions with reseachers in many different groups, including the following:
{% for item in site.data.collaborations %}

{% if item.link %}<b><a href="{{ item.link }}">{% endif %}{{ item.title }}{% if item.link %}</a></b>
{% endif %}
{% endfor %}


<h3>Facilities</h3>
The laboratory has access to the world-class research facilities of the University of Cambridge School of the Biological Sciences and the Department of Pathology, which provide state-of-the-art equipment, technical advice, and training. The facilities have an emphasis on quality and consistency and are vital in helping us deliver world-class research. Read more about [Research Facilities at the School of the Biological Sciences](https://www.bio.cam.ac.uk/facilities), and [Research Facilities at the Department of Pathology](https://www.path.cam.ac.uk/research/facilities). The following are facilities we make frequent use of:

{% for item in site.data.facilities %}
{% if item.link %}<b><a href="{{ item.link }}">{% endif %}{{ item.title }}{% if item.link %}</a>
</b>{% endif %}
{% endfor %}

<br />