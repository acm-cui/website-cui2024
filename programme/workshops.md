---
title: Workshops
label: Workshops
description: Workshops hosted at the ACM Conversational User Interfaces (CUI) !!conference.year!! conference.

maintainer: workshops
lastmod: page

menus:
  attend:
    text: Workshops
    title: Workshops hosted at CUI !!conference.year!!.
    weight: 1
    sep_before: true
  programme:
    text: Workshops
    title: Workshops hosted at CUI !!conference.year!!.
    weight: 11
---

CUI {{ site.conference.year }} is delighted to hosted four topical workshops at the conference this year. Attendance at workshops requires [conference and workshop registration]({{"/attend/registration/" | relative_url}}) prior to the conference. Each workshop may have its own criteria for attendance (e.g., the submission of a position paper), thus you are advised to check details posted by workshop organisers in advance of the conference.

{% for workshop in site.data.workshops %}

{% if forloop.index0 > 0 %}

<br>
{% endif %}

## {{ workshop.title }}
<em>{{ workshop.datetime }}</em> &bull; {% if workshop.url %}[Workshop Website]({{ workshop.url }} "{{ workshop.title}}"){% else %}Workshop Website TBC{% endif %}

{{ workshop.description}}

Organised by {{ workshop.organisers }}

{% endfor %}
