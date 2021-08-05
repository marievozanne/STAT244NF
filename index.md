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


- [course calendar](calendar.md),
- a [staff](staff.md) page,
- and a weekly [schedule](schedule.md).

Just the Class is built on top of [Just the Docs](https://github.com/pmarsceill/just-the-docs), making it easy to extend for your own special use cases while providing sane defaults for most everything else. This means that you also get:

- automatic [navigation structure](https://pmarsceill.github.io/just-the-docs/docs/navigation-structure/),
- instant, full-text [search](https://pmarsceill.github.io/just-the-docs/docs/search/) and page indexing,
- and a small but powerful set of [UI components](https://pmarsceill.github.io/just-the-docs/docs/ui-components) and authoring [utilities](https://pmarsceill.github.io/just-the-docs/docs/utilities).

## Getting Started

Getting started with Just the Class is simple.

1. Create a [new repository based on Just the Class](https://github.com/kevinlin1/just-the-class/generate).
1. Update `_config.yml` and `index.md` with your course information.
1. Configure a [publishing source for GitHub Pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages). Your course website is now live!
1. Edit and create `.md` [Markdown files](https://guides.github.com/features/mastering-markdown/) to add your content.

For a few open-source examples, see the following course websites and their source code.

- [CSE 390HA](https://courses.cs.washington.edu/courses/cse390ha/20au/) ([source code](https://gitlab.cs.washington.edu/cse390ha/20au/website)) is an example of a single-page website that centers modules.
- [CSE 143](https://courses.cs.washington.edu/courses/cse143/20au/) ([source code](https://gitlab.cs.washington.edu/cse143/20au/website)) hosts an entire online textbook with full-text search.
- [CSE 373](https://courses.cs.washington.edu/courses/cse373/21su/) ([source code](https://gitlab.cs.washington.edu/cse373-root/21su/website) is an example of a simple website combining Markdown pages with generated HTML files.

Share your website with us in the [show and tell discussion](https://github.com/kevinlin1/just-the-class/discussions/categories/show-and-tell)!

Continue reading to learn how to setup a development environment on your local computer. This allows you to make incremental changes without directly modifying the live website.
