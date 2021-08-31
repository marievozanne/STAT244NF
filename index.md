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

As we are all painfully aware, infectious disease can play a prominent role in our lives. Statistical and computational models serve a critical role in improving understanding of the progression and proliferation of infection in a population, as well as the impact of interventions in stopping the spread of disease. This course will be split into three sections: (1) epidemiological characteristics, which will include discussion of available data, descriptive summaries of data, and some regression-based methods for modeling infection characteristics; (2) compartmental models and corresponding simulations; (3) agent-based models and corresponding simulations. Many of our examples will be motivated by some of the most impactful epidemics and pandemics in recent history, including HIV/AIDS, Ebola, Zika, and COVID-19. We will make regular use of R statistical software in this class and work up to simulating infectious disease dynamics.

By the end of the course, you will be able to:

1. Define and estimate important epidemiology terms relating to infectious diseases.
2. Identify and estimate the effect of various risk factors for various infectious diseases through regression-based statistical models.
3. Represent and simulate infection spread through probabilistic compartmental models.
5. Simulate infection spread through agent-based models.
6. Explain the strengths and limitations of the modeling methods presented in this class.


<small>[Read more...]({{ site.baseurl }}{% link about.md %})</small>

{% for module in site.modules %}
{{ module }}
{% endfor %}


{% if site.announcements %}
{{ site.announcements.last }}
[Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}