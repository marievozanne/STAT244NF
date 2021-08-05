---
layout: home
title: "STAT 244NF"
nav_exclude: true
seo:
  type: Course
  name: Infectious Disease Modeling
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign overview = site.slides | where: "title", "Overview" | first %}
{{ overview.content }}

## Class Description

Infectious disease has plagued humanity since time immemorial. Statistical models serve a critical role in improving understanding of the progression and proliferation of infection in a population, as well as the impact of interventions in stopping the spread of disease. 

In this course, we will explore regression, compartmental and agent-based model approaches , which will be motivated by some of the most impactful epidemics and pandemics in recent history, including HIV/AIDS, Ebola, Zika, and COVID-19. 

By the end of the course, you will be able to:

1. Define important epidemiology terms relating to infectious diseases.
2. Identify and estimate the effect of various risk factors for various infectious diseases through statistical models.
3. Incorporate spatial dependence into statistical models.
4. Simulate infection spread through agent-based modeling.
5. Represent and make inference for infection spread through compartmental modeling.
6. Explain the strengths and limitations of the modeling methods presented in this class.


<small>[Read more...]({{ site.baseurl }}{% link about.md %})</small>

{% for module in site.modules %}
{{ module }}
{% endfor %}


{% if site.announcements %}
{{ site.announcements.last }}
[Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}