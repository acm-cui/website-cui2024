---
label: Provocations
description: Provocation papers at CUI !!conference.year!! explore controversial, risk-taking or nascent ideas that have the potential to spark debate and discussion at the conference.

splash_title: Provocations<br>at CUI !!conference.year!!

cta:
  text: Submit a provocation
  title: Submissions for the provocations track are open now
  link: /2024/submit/pcs/
  
track:
  chairs: provocations
  dates: provocations

menus:
  submit:
    title: Provocations
    alt: Information about submitting to the provocations track at CUI !!conference.year!!
    weight: 1
    is_track: true

lastmod: page
---

# Provocations at CUI 2024

Provocations at CUI are original and unpublished contributions. A compelling provocation is succinct yet potent, encapsulating a daring, thought-provoking idea or proposal. It should be a catalyst, igniting robust debate and stimulating a rich exchange of ideas among conference attendees. Provocations challenge the status quo, dare to push conventionality, and are willing to incite strong reactions or dissent. Through such provocations, we aim to unsettle comfortable paradigms, question established wisdom, and spur academic curiosity in the domain of conversational user interfaces. We encourage out-of-the-box or even controversial ideas to be proposed through provocation. Submissions addressing the theme of CUI 2024 of “Trustworthy Conversational Agents” are encouraged but not required. 

Late-breaking/non-provocative work should be submitted to the other tracks of CUI 2024 (either Posters or Demos are potentially applicable destinations).

Examples of previously successful provocation submissions at CUI can be found in the ACM Digital Library. Last year’s provocation papers were published as ["extended abstracts"](https://dl.acm.org/doi/proceedings/10.1145/3571884 'CUI 2023 proceedings').

## Key dates

{% for date in site.data.track_dates[page.track.dates] -%}
{{ date.label }}: {% if date.extended_date %}<strike>{{ date.date }}</strike> <strong>{{ date.extended_date }}</strong>{% else %}<strong>{{ date.date }}</strong>{% endif %}<br>
{%- endfor -%}

<em class="small"><br>All deadlines are at <a href="https://time.is/Anywhere_on_Earth" title="The current time in 'Anywhere on Earth'">23:59 Anywhere on Earth</a></em>

## The process

All submissions will proceed through the following process. Please contact the <a href="{{ site.data.oc['tracks']['roles'][page.track.chairs]['email'] }}" title="Contact the CUI {{ site.conference.year }} {{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }} if you have any questions">{{ site.data.oc['tracks']['roles'][page.track.chairs]['label'] }}</a> if you have any questions.

### 1. Prepare your paper

Submissions of provocations must be in English, in PDF format, anonymised using the [CHI anonymization policy](https://chi2024.acm.org/for-authors/presenting/papers/chi-anonymization-policy/ "CHI 2024 Anonymization Policy"), and approximately **3,000-3,500 words** words (including figures, tables, proofs, appendixes, and any other content excluding references and acknowledgments).

You must use the [ACM LaTeX or Word templates](https://www.acm.org/publications/proceedings-template "ACM templates for Microsoft Word and LaTeX") to prepare your submission.  LaTeX users may start their work by using the official ACM template available on [Overleaf](https://www.overleaf.com/latex/templates/acm-conference-proceedings-primary-article-template/wbvnghjbzwpc "ACM Primary Article Template templates on Overleaf"), which we strongly encourage. LaTeX users should have the following document class: <code>\documentclass[sigconf, screen, review, anonymous]{acmart}</code> for submission.

Word users must use [the one-column submission template](https://authors.acm.org/proceedings/production-information/preparing-your-article-with-microsoft-word "ACM submission template") and should be prepared to submit to TAPS approximately one week earlier than the stated camera-ready deadline. If accepted, word users may be required to reimplement their paper into the correct document format for the publishing process.

ACM’s CCS concepts and keywords are not required for submission and peer review but are required if your paper is accepted and published by the ACM.

### 2. Submit your paper

You should submit your paper to the [conference submission system]({{ "/submit/pcs/" | relative_url }} "CUI {{ site.conference.year }} submission system"). You must include your title, abstract, author details, and paper as a PDF. Your paper must be anonymised, or it may be desk rejected.

By submitting your article to an ACM Publication, you are hereby acknowledging that you and your co-authors are subject to all [ACM Publications Policies](https://www.acm.org/publications/policies "ACM Publications Policies and Procedures"), including [ACM's new Publications Policy on Research Involving Human Participants and Subjects](https://www.acm.org/publications/policies/research-involving-human-participants-and-subjects "https://www.acm.org/publications/policies/research-involving-human-participants-and-subjects"). Alleged violations of this policy or any ACM Publications Policy will be investigated by ACM and may result in a full retraction of your paper, in addition to other potential penalties, as per ACM Publications Policy.

We ask you to make sure that your submission is accessible for all users. To accomplish this, please follow the [SIGCHI Guide to an Accessible Submission](https://sigchi.org/conferences/author-resources/accessibility-guide/ "SIGCHI's guide to an Accessible Submission").

### 3. Await reviews

Each submission will be peer-reviewed by three expert reviewers under a double-anonymous refereed process (i.e., authors will not be revealed to reviewers, and all reviewers will be hidden from each other and authors). Papers for which there is a very high agreement among reviewers regarding recommendations for inclusion in the proceedings will receive acceptance decisions. Papers that provoke—even among reviewers—may be accepted.

### 4. Prepare your paper for publication

If your paper is accepted, you should de-anonymise it. You must include [CCS concepts](https://dl.acm.org/ccs "ACM Computing Classification System") and keywords for publication.

Programme Chairs will send information on how to ready your paper for the publishing process. Word users may be required to reimplement their paper, if accepted, into the correct document format for the publishing process, while LaTeX users will have to adjust their <code>documentclass</code>.

At least one author of each accepted paper must register for the conference, otherwise we cannot guarantee publication of your paper. Accepted papers will be archived in the <a href="http://dl.acm.org/" title="The ACM Digital Library">ACM Digital Library</a>.

You will receive an email from ACM to assign the rights for your paper, following which you will receive an email from "The ACM Publishing System" (TAPS), which will handle the generation of the final version of your paper. Accepted papers will be produced from LaTeX or Word source files into a single column HTML document and a two-column PDF for publication. We recommend all authors read ACM's guidance for [TAPS Best Practice](https://www.acm.org/publications/taps/taps-best-practices "The ACM Publishing System (TAPS) Best Practices").

Please ensure that you and your co-authors [obtain an ORCID ID](https://orcid.org/register "Register for an ORCID ID"), so you can complete the publishing process for your accepted paper. ACM has been involved in ORCID from the start and we have recently [made a commitment to collect ORCID IDs from all of our published authors](https://authors.acm.org/author-resources/orcid-faqs "ACM committment to collect ORCID IDs from all authors"). The collection process has started and will roll out as a requirement throughout 2022. We are committed to improve author discoverability, ensure proper attribution and contribute to ongoing community efforts around name normalization; your ORCID ID will help in these efforts.

All ACM publications follow the [Green Open Access route by default](https://www.acm.org/publications/openaccess#green "Details on ACM's Green Open Access policies"), although authors have the opportunity to independently pay a fee for [Gold Open Access](https://www.acm.org/publications/openaccess#oapricing "Details on Gold Open Access pricing for ACM publications"). The total fee payable depends on the author(s) ACM membership status.

### 5. Present your work

Authors will be given the opportunity to present their posters at CUI {{ site.conference.year }}. The specific details of this presentation will be provided closer to the conference.

## Questions?

<p>
{%- for group in site.data.oc -%}
{%- for role in group[1]['roles'] -%}
{%- if role[0] == page.track.chairs -%}
  If you have any questions, please contact the <a href="{{ role[1].email }}" title="Send an email to the CUI {{ site.conference.year }} {{ role[1].label }}">{{ role[1].label }}</a>, 
  {% assign use_and = role[1]['people'] | size | plus: -1 -%}
  {%- for person in role[1]['people'] -%}
      {{- person.name -}}
      {%- if forloop.index == use_and %} and {% else -%}{%- unless forloop.last %}, {% endunless -%}{%- endif -%}
  {%- endfor %} for support.
  {%- break -%}
{%- endif -%}
{%- endfor -%}
{%- endfor -%}
</p>


