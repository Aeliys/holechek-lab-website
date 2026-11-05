---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

The Holechek Laboratory is built on the premise that good science requires
people with different training, perspectives, and questions working in the
same room. Our team combines expertise in cell biology, biostatistics,
computational analysis, and clinical science.

We recruit actively and intentionally. First-generation college students,
online students, transfer students, and researchers entering without
traditional laboratory preparation are central to our team and our training
philosophy. We carry this commitment forward through active participation in
the SOLUR and iSTEM SOLUR Prep programs in the School of Life Sciences at
Arizona State University.

{% comment %}
  HOW TO PLACE SOMEONE ON THIS PAGE
  Each person has a file in the _members folder. Two fields decide where
  they appear:
    role:  principal-investigator, phd, undergrad, ata, ambassador, alum
           (controls the small icon on their photo; see _data/types.yaml)
    group: graduate, undergraduate, ambassador, immersion, alumni
           (controls which section below they are listed in)
  A section is hidden automatically until at least one person is in it.
{% endcomment %}

{% assign people = site.members %}

{% include section.html %}

## Principal Investigator

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}

{% assign group_members = people | data_filter: "group == 'graduate'" %}
{% if group_members.size > 0 %}

{% include section.html %}

## Graduate Students

Our graduate students lead independent projects and mentor undergraduate
researchers, often across both bench and computational work.

{% include list.html data="members" component="portrait" filter="group == 'graduate'" %}

{% endif %}

{% assign group_members = people | data_filter: "group == 'undergraduate'" %}
{% if group_members.size > 0 %}

{% include section.html %}

## Undergraduate Researchers

Our undergraduate researchers include students at multiple stages, from those
completing independent research projects to students in their first semester
of structured lab experience through iSTEM SOLUR Prep. All are full members of
the lab community.

{% include list.html data="members" component="portrait" filter="group == 'undergraduate'" %}

{% endif %}

{% assign group_members = people | data_filter: "group == 'ambassador'" %}
{% if group_members.size > 0 %}

{% include section.html %}

## All of Us Ambassadors

Dr. Holechek serves as Lead Ambassador for the
[All of Us Research Program](https://allofus.nih.gov/) at ASU. Our ambassadors
share information about the program with students and community members and
help connect researchers with this nationally diverse dataset.

{% include list.html data="members" component="portrait" filter="group == 'ambassador'" %}

{% endif %}

{% assign group_members = people | data_filter: "group == 'immersion'" %}
{% if group_members.size > 0 %}

{% include section.html %}

## Lab Immersion Instructional Team

Our immersion instructional team runs the hands-on research immersion weeks
that give online undergraduate and master's students laboratory experience
they would not otherwise get. Team members teach techniques, guide student
teams through experiments, and create learning materials such as talks and
videos.

{% include list.html data="members" component="portrait" filter="group == 'immersion'" %}

{% endif %}

{% assign group_members = people | data_filter: "group == 'alumni'" %}
{% if group_members.size > 0 %}

{% include section.html %}

## Lab Alumni

{% include list.html data="members" component="portrait" filter="group == 'alumni'" %}

{% endif %}

{% include section.html %}

## Join the Lab

We welcome students from every entry point, including online students and
students with no prior research experience. Most students join through the
[SOLUR program](https://sols.asu.edu/research/solur) or iSTEM SOLUR Prep.

{%
  include button.html
  link="contact"
  text="Get in touch"
  icon="fa-solid fa-arrow-right"
  flip=true
%}

{% comment %}
  GROUP PHOTOS
  When you have group photos, add them to the images folder and replace the
  file names below, then delete the comment tags around this block.

  {% include section.html %}

  ## Group Photos

  {% capture content %}
  {% include figure.html image="images/group-photo-1.jpg" %}
  {% include figure.html image="images/group-photo-2.jpg" %}
  {% include figure.html image="images/group-photo-3.jpg" %}
  {% endcapture %}

  {% include grid.html style="square" content=content %}
{% endcomment %}
