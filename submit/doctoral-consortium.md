---
label: Doctoral Consortium
description: The CUI !!conference.year!! Doctoral Consortium is designed to allow PhD students in the field of HCI and Conversational User Interfaces to present and share their work, and receive feedback, through an interactive workshop.

splash_title: Doctoral Consortium<br>at CUI !!conference.year!!

cta:
  text: Apply
  title: Applications for the CUI 2024 are open now Doctoral Consortium
  link: mailto:cui2024-dc@cui.acm.org
  
track:
  chairs: dc
  dates: doctoral_consortium

menus:
  submit:
    text: Doctoral Consortium
    title: Information about applying to the CUI !!conference.year!! doctoral consortium.
    weight: 5
    is_track: true

lastmod: page
---

# Doctoral Consortium

The CUI {{ site.conference.year }} Doctoral Consortium is a half-day session where doctoral students of conversational user interfaces can discuss their research with other students and experts within the field. Doctoral work is important to our rapidly advancing area of research, and we very much look forward to making the Doctoral Consortium a meeting place for students in the field.

## Key dates

{% for date in site.data.track_dates[page.track.dates] -%}
{{ date.label }}: {% if date.extended_date %}<strike>{{ date.date }}</strike> <strong>{{ date.extended_date }}</strong>{% else %}<strong>{{ date.date }}</strong>{% endif %}<br>
{%- endfor -%}

<em class="small"><br>All deadlines are at <a href="https://time.is/Anywhere_on_Earth" title="The current time in 'Anywhere on Earth'">23:59 Anywhere on Earth</a></em>

## The process

All demo papers will proceed through the following process. Please contact the <a href="{{ site.data.oc['tracks']['roles'][page.track.chairs]['email'] }}" title="Contact the CUI {{ site.conference.year }} {{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }} if you have any questions">{{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }}</a> if you have any questions.

### 1. Prepare your application

Students are invited to submit an application in extended abstract format for participation.

You must use the [ACM LaTeX or Word templates](https://www.acm.org/publications/proceedings-template "ACM templates for Microsoft Word and LaTeX") to prepare your submission.  LaTeX users may start their work by using the official ACM template available on [Overleaf](https://www.overleaf.com/latex/templates/acm-conference-proceedings-primary-article-template/wbvnghjbzwpc "ACM Primary Article Template templates on Overleaf"), which we strongly encourage. LaTeX users should have the following document class: <code>\documentclass[sigconf, screen, review]{acmart}</code> for submission.

Word users should use [the double-column "Interim Template"](https://www.acm.org/publications/proceedings-template#h-interim-template "ACM Interim Template for submissions").

The application should be submitted as a single pdf file (max. 2 pages) outlining a research statement which contains the following: 
 
1. A summary of the applicant's research topic  
2. Answers to the following questions:  
	a. How far you are in your PhD?  
	b. What is the motivation for this research?  
	c. What is the expected contribution to the field?  
	d. What progress have you made so far?  
	e. What would you like to learn and discuss during the Doctoral Consortium? 

### 2. Submit your application

You should submit your application by email to [cui2024-dc@cui.acm.org](mailto:cui2024-dc@cui.acm.org), making sure to include your full name, affiliation, and preferred contact email in the submission email text, as well as your extended abstract.

### 3. Selection process – curated

Doctoral Consortium participants will be selected on the basis of their research statement through a curated process where the aim is to establish a participant group with complementary research interests and aims for participation. We aim for an inclusive selection process.

### 4. Present and discuss your PhD

As well as taking part in the Doctoral Consortium discussions and presentations, accepted participants are furthermore encouraged to present their thesis as a poster. This poster shall be presented alongside the posters from the poster session at the main conference so that students may receive feedback from conference attendees who are not part of the Doctoral Consortium.

The CUI 2024 posters chairs will send information about the poster format upon acceptance as the Doctoral Consortium will use the same format.

## Questions?

{% for group in site.data.oc -%} {%- for role in group[1]['roles'] -%} {%- if role[0] == page.track.chairs -%} If you have any questions, please contact the [{{ role[1].label }}]({{ role[1].email }}), {% assign use_and = role[1]['people'] | size | plus: -1 -%} {%- for person in role[1]['people'] -%} {{- person.name -}} {%- if forloop.index == use_and %}{% if forloop.length > 2 %},{% endif %} and {% else -%}{%- unless forloop.last %}, {% endunless -%}{%- endif -%} {%- endfor %}, for support. {%- break -%} {%- endif -%} {%- endfor -%} {%- endfor -%}
