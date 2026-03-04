---
permalink: /research/
title: "Research"
toc: true
toc_label: "On This Page"
toc_icon: "list"
toc_sticky: true
---


## Critical biology is invisible to static structures

Function arises from conformational ensembles — but is interpreted using single, static structures. The biggest questions in human health demand that we understand not only what molecules look like, but how they move.

![diffuse scattering signals](/assets/images/diffuse_signals.png){:style="max-height:300px; display: block; margin-left: auto; margin-right: auto;"}

To unlock the next frontier of advances, we need new methods, more experimental data, and better ways to model and encode protein dynamics. By openly building tools and methods, we engage the entire community to contribute, enabling the scale and diversity of data needed to uncover biological principles.

## Our Research Questions

**01** &nbsp; What data are we missing, and how do we accelerate the technologies to capture it?

**02** &nbsp; Where will dynamic structural data have the greatest impact in revealing biological function?

**03** &nbsp; How do we build enabling tools that empower everyone — not just experts — to leverage dynamic structural information?

**04** &nbsp; How do we disseminate our tools and data to maximize scientific impact?

---

*What makes a designed enzyme functional?*

---

![MD simulated diffuse scattering](/assets/images/20250805_Mac1_diffuse_crop.png){:style="max-height:300px; display: block; margin-left: auto; margin-right: auto;"}

## We are working to

{% assign interests = site.research | sort: "index" %}

{% for interest in interests %}
### {{ interest.name }}

{% assign parity = interest.index | modulo:2 %}
{% if parity == 0 %}
{% assign alignment = "right" %}
{% else %}
{% assign alignment = "left" %}
{% endif %}

![{{interest.image_alt}}]({{interest.image}}){:style="float: {{alignment}}; object-fit: contain; width: 35%; max-height: 50em; margin-left: 1em; margin-right: 1em;"}

{{ interest.content }}
{% endfor %}
