---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

For a quicker response on homework or project help, please ask on EdStem rather than emailing staff members individually. On EdStem, all staff members can see your question and answer it.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Hampton Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Google Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Google Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign career_coach = site.staffers | where: 'role', 'Career Coach' %}
{% assign num_teaching_assistants = career_coach | size %}
{% if num_teaching_assistants != 0 %}

## Career Coach

{% for staffer in career_coach %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign curriculum_collab = site.staffers | where: 'role', 'Curriculum Developer' %}
{% assign num_teaching_assistants = curriculum_collab | size %}
{% if num_teaching_assistants != 0 %}
## Curriculum Collaborator

{% for staffer in curriculum_collab %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign u_program_specialist = site.staffers | where: 'role', 'University Program Specialist' %}
{% assign num_teaching_assistants = u_program_specialist | size %}
{% if num_teaching_assistants != 0 %}
## Google University Program Specialist

{% for staffer in u_program_specialist %}
{{ staffer }}
{% endfor %}
{% endif %}

<!-- ## Google TAs

{% assign google_teaching_assistants = site.staffers | where: 'role', 'GoogleTA' %}
{% for staffer in google_teaching_assistants %}
{{ staffer }}
{% endfor %} -->

<!-- {% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %} -->
<!-- ## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %} -->
