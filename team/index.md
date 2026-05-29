---
title: Team
nav:
  order: 3
  tooltip: About our team
---

## {% include icon.html icon="fa-solid fa-users" %}Team

The Holechek laboratory is built on the premise that good science requires
people with different training, perspectives, and questions working in the
same room. Our team combines expertise in cell biology, biostatistics,
computational analysis, and clinical science.

We recruit actively and intentionally. First-generation college students,
online students, transfer students, and researchers entering without
traditional laboratory preparation are are central to our team and training philliosphopy. We continue this commitment through active participation in both the SOLUR and SOLUR PREP programs through the School of Life Sciences at Arizona State University.

# # {% include icon.html icon="fa-solid fa-users" %}

## Principal Investigator

{% include list.html data="members" component="portrait" filter="role == 'pi'" %}

{% include section.html %}

## Graduate Students

{% include list.html data="members" component="portrait" filter="group == 'graduate'" %}

{% include section.html %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

## Undergraduate Researchers

Our undergraduate researchers include students at multiple stages, from those
completing independent research projects to students in their first semester
of structured lab experience through SOLUR PREP. All are full members of the
lab community.

{% include list.html data="members" component="portrait" filter="group == 'undergraduate'" %}

## All of Us Ambassadors

## Lab Immersion Instructional Team

{% include list.html data="members" component="portrait" filter="group == 'immersion'" %}

## Lab Alumni

{% include list.html data="members" component="portrait" filter="group == 'alumni'" %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

## Group Photos

## Funding

{% endcapture %}

{% include grid.html style="square" content=content %}
