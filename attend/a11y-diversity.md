---
title: Accessibility and Diversity
label: Accessibility and Diversity
description: Information about how we're supporting accessibility and diversity at CUI !!conference.year!!.

maintainer: diversity
lastmod: page

registration_open: false

menus:
  attend:
    text: Accessibility and Diversity
    title: Information about how we're supporting accessibility and diversity at CUI
    weight: 6
    sep_before: true
---

CUI {{ site.conference.year }} strives to be an inclusive and accessible conference, and we will do our best to accommodate requests for special assistance. Information will be posted here as we develop our plans for the conference, to help you decide whether the conference will be accessible to you. Please get in touch with us if your question is not answered here, or if the conference arrangements as described are not enough to allow you to attend.

{% for group in site.data.oc %}
	{% for role in group[1]['roles'] %}
		{%- if role[0] == page.maintainer %}
<p>The {{ role[1].label }} are progressively assembling this information. If you have questions or wish to raise a point regarding our efforts to ensure all attendees can participate, please contact us by <a href="{{ role[1].email }}" title="Email address for the CUI {{ site.conference.year }} {{ role[1].label }}">email at {{ role[1].email | replace: "mailto:", "" }}</a>. Rest assured, we will work with you to make the conference accessible.</p>
		{% break %}
		{% endif %}
	{% endfor %}
{% endfor %}

## Pronouns
Per CUI’s commitment to diversity, inclusion, and equity, we wish all attendees to indicate their pronouns to promote a safe, welcoming environment. This information will be included on your CUI {{ site.conference.year }} badge and in the online attendee profile of the virtual platform to foster dignity, courtesy, understanding, and mutual respect during interactions throughout the conference. Providing/displaying your pronoun on your badge is not mandatory.

## How do I communicate accessibility needs to organisers?
The Diversity & Accessibility chairs aims to ensure the conference is accessible to everyone. When you register for the conference, there will be questions for you to answer about your needs. Please complete these to indicate anything that will help make the conference accessible.

Possible requests include but are not limited to: sign language interpretation, note taker, assistive listening device, captioning, description (for slides, overheads or videos), and so on. The Diversity & Accessibility chairs will follow up with requests. You can contact them directly at any time by {% for group in site.data.oc %}{% for role in group[1]['roles'] %}{%- if role[0] == page.maintainer %}<a href="{{ role[1].email }}" title="Email address for the CUI {{ site.conference.year }} {{ role[1].label }}">emailing us</a>{% break %}{% endif %}{% endfor %}{% endfor %}.

Please be aware that some accommodations may be difficult to provide at short notice, and we may only be able to accommodate some requests.

## Will sign language interpretation be available?
If you request sign language interpretation in your conference registration, we will strive to provide interpretation for all conference presentations and events, including informal conversations. Please register your request before the 1st June {{ site.conference.year }} by {% for group in site.data.oc %}{% for role in group[1]['roles'] %}{%- if role[0] == page.maintainer %}<a href="{{ role[1].email }}" title="Email address for the CUI {{ site.conference.year }} {{ role[1].label }}">emailing us</a>{% break %}{% endif %}{% endfor %}{% endfor %}. We will try to accommodate requests made after this date but with no guarantees. You may also bring your interpreter to the event. Please reach out to the Diversity & Accessibility chairs to set this up. 

## What are the public transport options for getting to the conference venue?
For information about the public transport options for getting to the conference venue, please see [travel information for CUI]({{ "/attend/travel-to-cui/" | relative_url }} "Travel information for CUI {{ site.conference.year }}").

## I have another question.

{% for group in site.data.oc %}
	{% for role in group[1]['roles'] %}
		{%- if role[0] == page.maintainer %}
<p>If you have other questions about accessibility at CUI {{ site.conference.year }}, please contact the {{ role[1].label }} by <a href="{{ role[1].email }}" title="Email address for the CUI {{ site.conference.year }} {{ role[1].label }}">emailing us</a>.</p>
		{% break %}
		{% endif %}
	{% endfor %}
{% endfor %}
