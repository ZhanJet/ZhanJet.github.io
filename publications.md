---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "**Zhangjie Tu**, Tianwei Zhang, Lei Yan, Tin lun Lam"
    title: "Whole-Body Control for Velocity-Controlled Mobile Collaborative Robots Using Coupling Dynamic Movement Primitives"
    month: "**submitted**"
    year: ""
    journal: "IROS2022"
    url: "https://arxiv.org/abs/2203.03296"
#  - author: "**Zhangjie Tu**, Peng Lu"
#    title: "Model-based Disturbance Observation and Rejection for Quadrotors Inputted with Wrench Command"
#    month: "**in prep**"
#    year: ""
#    booktitle: "Technical Report"
#    url: ""

  - author: "Zhiwei Hou, Peng Lu, **Zhangjie Tu**"
    title: "Nonsingular Terminal Sliding Mode Control for a Quadrotor UAV with a Total Rotor Failure"
    month: "March"
    year: "2020"
    journal: "Aerospace Science and Technology"
    url: "https://www.sciencedirect.com/science/article/abs/pii/S1270963819316414"

  - author: "**Zhangjie Tu**, Lixin Wang, Junping Chen"
    title: "Assessment of Go-around Climb Gradient for Civil Aircraft Based on Digital Virtual Flight"
    month: "February"
    year: "2017"
    journal: "Journal of Beijing University of Aeronautics & Astronautics"
    url: "https://bhxb.buaa.edu.cn/EN/10.13700/j.bh.1001-5965.2016.0879"
---
## Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}

- {% if pub.url %} [{{pub.title}}]({{pub.url}}).
  {% else %} {{pub.title}}.
  {% endif %}{% if pub.type %}({{pub.type}})
  {% endif %}<br>
  {{pub.author}}.<br>
  {% if pub.type == 'Technical Report' %}{{pub.number}}
  {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
  {% if pub.address %}{{pub.address}}.
  {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
  {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
  {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
  {% endif %}
  {% endunless %}
  {% endfor %}

## Patents

* [Synchronous calibration method for zero-offset of F/T sensor and load parameter, CN108716962A.](https://www.patent9.com/patent/201810442844.X.html)
* [Simulation and design platform for industrial robot design and verification, CN108595888A.](https://www.patent9.com/patent/201810442827.6.html)
