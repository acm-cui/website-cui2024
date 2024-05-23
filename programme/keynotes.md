---
title: Conference Keynotes
label: Conference keynotes
description: >
  CUI !!conference.year!! will feature a keynote from distinguished academic: Simon King from the University of Edinburgh.

maintainer: general
lastmod:
  type: data
  file: keynotes.yml

menus:
  programme:
    text: Keynotes
    title: The CUI !!conference.year!! conference keynotes
    weight: 0
---

{% for keynote in site.data.keynotes %}

<h2>{{ keynote.speaker }}: {{ keynote.title }}</h2>

<div class="d-flex flex-md-row flex-column">
	<div class="flex-grow-1 pe-3">
	  <p>{{ keynote.abstract }}</p>
	  <p><em>{{ keynote.biography }}</em></p>
  </div>
  <img src="{{ "/assets/img/keynotes/" | append: keynote.image | relative_url }}" alt="A photograph of {{ keynote.speaker }}" title="{{ keynote.speaker }}" class="flex-grow-0 align-self-start ml-md-3 mr-md-0 mx-auto mt-md-0 mt-3 rounded shadow">
</div>

{% endfor %}
