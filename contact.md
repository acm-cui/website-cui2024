---
label: Contact
description: Contact details for ACM CUI !!conference.year!!.
lastmod: page

title: Contact us

menu:
  main:
    text: Contact
    title: Contact the ACM CUI !!conference.year!! General Chairs
    weight: 10
---


<p>
{%- for group in site.data.oc -%}
    {%- for role in group[1]['roles'] -%}
        {% if role[1]['contact'] -%}
			If you need any help or have questions regarding the conference, please do not hesitate to get in touch with the <a href="{{ role[1].email }}" title="Send an email to the CUI {{ site.conference.year }} {{ role[1].label }}">CUI {{ site.conference.year }} {{ role[1].label }}</a>: <br>
			{% assign use_and = role[1]['people'] | size | plus: -1 -%}
			{%- for person in role[1]['people'] -%}
				{{- person.name -}}
				{%- if forloop.index == use_and %}, and {% else -%}{%- unless forloop.last %}, {% endunless -%}{%- endif -%}
			{%- endfor -%}.
            {%- break -%}
        {%- endif -%}
    {%- endfor -%}
	{%- break -%}
{%- endfor -%}
</p>