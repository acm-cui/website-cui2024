---
label: Posters
description: Posters at CUI !!conference.year!! are short papers that present early-stage research and late-breaking work in the field of Conversational User Interfaces.

splash_title: Posters<br>at CUI !!conference.year!!

cta:
  text: Submit a poster
  title: Submissions for the posters track are open now
  link: /2024/submit/pcs/
  
track:
  chairs: postersdemos
  dates: short_papers

menus:
  submit:
    text: Posters
    title: Information about submitting to the posters track at CUI !!conference.year!!
    weight: 2
    is_track: true

lastmod: page
---

# Posters

We invite the submission of posters from a broad range of disciplines, including human-computer interaction, computer science, engineering, speech technology, linguistics, psychology, cognitive sciences, sociology, and other cognate disciplines. 

Posters are short papers that present early-stage research and late-breaking work in the field of Conversational User Interfaces. This track is suitable for shorter, original contributions that do not meet the length requirements or depth required for the Papers track. Submissions can include preliminary results, short prequels to or follow-ups of larger studies, early student research, and other research that is better suited to an interactive discussion format. For the submission and review process, you should write an extended abstract that summarizes the content you wish to present in your poster. If accepted, we will invite you to present your work at CUI 2024, with your extended abstract published in the conference proceedings.

Examples of previously successful poster submissions at CUI can be found in the ACM Digital Library. Last year’s posters were published as ["demonstration"](https://dl.acm.org/doi/proceedings/10.1145/3571884 'CUI 2023 proceedings') in the posters and demos session.

## Key dates

{% for date in site.data.track_dates[page.track.dates] -%}
{{ date.label }}: {% if date.extended_date %}<strike>{{ date.date }}</strike> <strong>{{ date.extended_date }}</strong>{% else %}<strong>{{ date.date }}</strong>{% endif %}<br>
{%- endfor -%}

<em class="small"><br>All deadlines are at <a href="https://time.is/Anywhere_on_Earth" title="The current time in 'Anywhere on Earth'">23:59 Anywhere on Earth</a></em>

## The process

All submissions will proceed through the following process. Please contact the <a href="{{ site.data.oc['tracks']['roles'][page.track.chairs]['email'] }}" title="Contact the CUI {{ site.conference.year }} {{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }} if you have any questions">{{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }}</a> if you have any questions.

### 1. Prepare your extended abstract

Submissions of extended abstracts for posters must be in English, in PDF format, anonymised using the [CHI anonymization policy](https://chi2024.acm.org/for-authors/presenting/papers/chi-anonymization-policy/ "CHI 2024 Anonymization Policy"), and approximately **3,000 words** words (including figures, tables, proofs, appendixes, and any other content excluding references and acknowledgments).

You must use the [ACM LaTeX or Word templates](https://www.acm.org/publications/proceedings-template "ACM templates for Microsoft Word and LaTeX") to prepare your submission. We encourage the use of LaTeX and the official ACM template on [Overleaf](https://www.overleaf.com/latex/templates/acm-conference-proceedings-primary-article-template/wbvnghjbzwpc "ACM Primary Article Template templates on Overleaf"). LaTeX users must employ the following document class for submission: <code>\documentclass[manuscript,screen,review,anonymous]{acmart}</code> for submission.

Word users must use [the one-column submission template](https://authors.acm.org/proceedings/production-information/preparing-your-article-with-microsoft-word "ACM submission template") and should be prepared to submit to TAPS ***approximately one week earlier*** than the stated camera-ready deadline.

ACM’s CCS concepts and keywords are not required for submission and peer review but are required if your paper is accepted and published by the ACM.

### 2. Submit your extended abstract

You should submit your extended abstract and video to the [conference submission system]({{ "/submit/pcs/" | relative_url }} "CUI {{ site.conference.year }} submission system"). You must include your title, abstract, author details, and extended abstract as a PDF. Your extended abstract must be anonymised, or it may be desk rejected.  Please follow the [SIGCHI Guide to an Accessible Submission](https://sigchi.org/conferences/author-resources/accessibility-guide/  "SIGCHI's guide to an Accessible Submission") to make your submission accessible for all users. Submitting your article to an ACM Publication acknowledges that you and your co-authors are subject to all [ACM Publications Policies](https://www.acm.org/publications/policies "ACM Publications Policies and Procedures").

### 3. Await reviews

Each submission will be peer reviewed by three expert reviewers under a refereed process under a double-anonymous process (i.e., authors will not be revealed to reviewers, and all reviewers will be hidden from each other and authors). Extended abstracts for which there is a very high agreement among reviewers regarding recommendations for inclusion in the proceedings will receive early acceptance decisions and will be conditionally accepted, pending the integration of any changes requested through the review process.

### 4. Prepare your paper for publication

If your extended abstract is accepted, you should de-anonymise it. You must include [CCS concepts](https://dl.acm.org/ccs "ACM Computing Classification System") and keywords for publication. At least one author of each accepted paper must register for the conference. Otherwise, we cannot guarantee the publication of your paper. Accepted demo extended abstracts will be archived in the <a href="http://dl.acm.org/" title="The ACM Digital Library">ACM Digital Library</a>.

You will receive an email from ACM to assign the rights for your paper, following which you will receive an email from "The ACM Publishing System" (TAPS), which will handle the generation of the final version of your paper. Accepted papers will be produced from LaTeX or Word source files into a single column HTML document and a two-column PDF for publication. We recommend all authors read ACM's guidance for [TAPS Best Practice](https://www.acm.org/publications/taps/taps-best-practices "The ACM Publishing System (TAPS) Best Practices").

Please ensure that you and your co-authors [obtain an ORCID ID](https://orcid.org/register "Register for an ORCID ID") to complete the publishing process for your accepted paper. Your paper will be published in the ACM CUI Proceedings in the [ACM Digital Library](http://dl.acm.org/). [SIGCHI](https://sigchi.org) participates in the [ACM Open Table of Contents (OpenTOC)](https://www.acm.org/publications/openaccess) service, which means papers will be freely available from this website for the first year after publication. Publications are [Green Open Access](https://www.acm.org/publications/openaccess#h-green-open-access) by default but can be upgraded to [Gold Open Access](https://www.acm.org/publications/openaccess#h-gold-open-access-publication) for a fee.

### 5. Present your work

Authors will be given the opportunity to present their posters at CUI {{ site.conference.year }}. The specific details of this presentation will be provided closer to the conference.

## Questions?

{% for group in site.data.oc -%} {%- for role in group[1]['roles'] -%} {%- if role[0] == page.track.chairs -%} If you have any questions, please contact the [{{ role[1].label }}]({{ role[1].email }}), {% assign use_and = role[1]['people'] | size | plus: -1 -%} {%- for person in role[1]['people'] -%} {{- person.name -}} {%- if forloop.index == use_and %}{% if forloop.length > 2 %},{% endif %} and {% else -%}{%- unless forloop.last %}, {% endunless -%}{%- endif -%} {%- endfor %}, for support. {%- break -%} {%- endif -%} {%- endfor -%} {%- endfor -%}

