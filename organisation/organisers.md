---
label: Organising Committee
description: The Organising Committee for the !!conference.year!! Conversational User Interfaces conference.
lastmod:
  type: data
  file: oc.yml

title: Organising Committee

menus:
  organisers:
    text: Organising Committee
    title: Volunteers leading the organisation and running of Conversational User Interfaces !!conference.year!!
    weight: 0
---

<p class="text-center">
    The following people have volunteered their time to assist in the organisation of ACM CUI {{ site.conference.year }}.
</p>

{% for group in site.data.oc %}
    {% assign num_roles_chairs = group[1]['roles'] | size %}
    {% assign half_num_roles_chairs = num_roles_chairs | plus: 1  | divided_by: 2%}

<div class="text-center">
    <div class="mb-0">
        <h2>{{ group[1].label }}</h2>
        {% for role in group[1]['roles'] %}
        <h3>{{ role[1].label }}{%- if role[1].contact %} <a href="{{ role[1].email }}" title="Send an email to the CUI {{ site.conference.year }} {{ role[1].label }}">
            <picture>
                <source srcset="{{ site.baseurl }}/assets/img/envelope-fill-w.svg" media="(prefers-color-scheme: dark)" width="30px" height="auto"/>
                <img src="{{ site.baseurl }}/assets/img/envelope-fill.svg" width="30px" height="auto"/>
            </picture>
        </a>{% endif %}</h3>
        <ul class="list-unstyled d-inline-block" style="min-width: 400px">
            {% for people in role[1]['people'] %}
            <li class="d-flex my-4 align-items-center mx-auto">
                <div class="flex-shrink-0">
                        {%- if people.image %}
                        {%- assign image = people.image -%}
                        {%- else -%}
                        {%- assign image = 'noimage.jpg' -%}
                        {%- endif -%}
                    <img src="{{ "/assets/img/oc/" | append: image | relative_url }}" height="auto" width="100" style="border-radius:50%" alt="A photo of {{ people.name }}" title="{{ people.name }}">
                </div>
                <div class="flex-grow-1 ms-3 text-start">
                        {{ people.name }}<br><span class="text-muted small">{{ people.position }}<br>{{ people.institution }}, {{ people.country }}</span>
                </div>
            </li>
            {% endfor %}
        </ul>
        {% endfor %}
    </div>
</div>

    {% unless forloop.last %}

 ---

    {% endunless %}

{% endfor %}
