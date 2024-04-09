---
label: Registration information
description: Details about registration for the ACM Conversational User Interfaces (CUI) !!conference.year!! conference.

title: Registration
splash_title: Register for CUI !!conference.year!!

cta:
  text: Registration opens soon
#  text: Register now
#  title: Registration for ACM CUI is open now
#  link: https://cvent.me/A8XxdO

registration_open: false

menus:
  attend:
    text: Registration
    title: Registration details for CUI !!conference.year!!.
    weight: 0
---

CUI {{ site.conference.year }} will be an in-person conference, and as such, our registration fees reflect running an in-person event. 

{% if page.registration_open %}
Registration for CUI {{ site.conference.year }} is now open.
{% else %}
We hope to open registration for CUI {{ site.conference.year }} very soon.
<!-- Online registration has now closed, and you must register on-site.-->
{% endif %}

Authors with papers accepted must register by **9th June 2024**. At least one author of each accepted paper, poster, DC, or demo must be registered to attend the conference in person. Any submission without a corresponding registration may be withheld from publication. We will support remote presentations only in an emergency (i.e., VISA being denied). 
Please ensure you register at the correct rate—if you do not, you will be liable to pay the difference. You can revise your registration online up to one week before the conference.


### Registration fees

There are four different rates for registration at CUI {{ site.conference.year }} in-person and two different registration deadlines:

* Early registration closes on **8th June 2024**
* Late registration closes on **8th July 2024**

<table class="registration-rates mx-auto mt-4 mb-3 text-center d-md-table d-none">
	<thead class="border-bottom">
		<th></th>
		<th class="px-3 pb-3 align-top text-center">Student<br>Non-member</th>
		<th class="px-3 pb-3 align-top text-center">Student<br>Member</th>
		<th class="px-3 pb-3 align-top text-center">Professional<br>Non-member</th>
		<th class="px-3 pb-3 align-top text-center">Professional<br>Member</th>
	</thead>
	<tbody>
		<tr class="mb-3 ">
				<td class="pe-3 py-3"><strong>Early</strong></td>
				<td class="py-3">€500</td>
				<td class="py-3">€400</td>
				<td class="py-3">€700</td>
				<td class="py-3">€600</td>
		</tr>
		<tr class="pb-3">
				<td class="pe-3 py-3"><strong>Late</strong></td>
				<td class="py-3">€550</td>
				<td class="py-3">€450</td>
				<td class="py-3">€800</td>
				<td class="py-3">€700</td>
		</tr>
		<tr class="pb-3 border-bottom">
				<td class="pe-3 py-3"><strong>On-site</strong></td>
				<td class="py-3">€600</td>
				<td class="py-3">€500</td>
				<td class="py-3">€900</td>
				<td class="py-3">€800</td>
		</tr>
	</tbody>
</table>

<table class="registration-rates w-100 mx-auto border-bottom mt-4 text-center d-md-none d-table">
	<thead class="border-bottom">
		<th></th>
		<th class="px-3 py-3 align-top text-center">Student<br>Non-member</th>
		<th class="px-3 py-3 align-top text-center">Student<br>Member</th>
	</thead>
	<tbody>
		<tr class="mb-3 ">
			<td class="pe-3 py-3"><strong>Early</strong></td>
			<td class="py-3">€500</td>
			<td class="py-3">€400</td>
		</tr>
		<tr class="pb-3">
			<td class="pe-3 py-3"><strong>Late</strong></td>
			<td class="py-3">€550</td>
			<td class="py-3">€450</td>
		</tr>
		<tr class="pb-3 border-bottom">
			<td class="pe-3 py-3"><strong>On-site</strong></td>
			<td class="py-3">€600</td>
			<td class="py-3">€500</td>
		</tr>
	</tbody>
</table>

<table class="registration-rates border-top w-100 mx-auto mt-1 mb-3 text-center  d-md-none d-table">
	<thead class="border-bottom">
		<th></th>
		<th class="px-3 py-3 align-top text-center">Professional<br>Non-member</th>
		<th class="px-3 py-3 align-top text-center">Professional<br>Member</th>
	</thead>
	<tbody>
		<tr class="mb-3">
			<td class="pe-3 py-3"><strong>Early</strong></td>
			<td class="py-3">€700</td>
			<td class="py-3">€600</td>
		</tr>
		<tr class="pb-3">
			<td class="pe-3 py-3"><strong>Late</strong></td>
			<td class="py-3">€800</td>
			<td class="py-3">€700</td>
		</tr>
		<tr class="pb-3 border-bottom">
			<td class="pe-3 py-3"><strong>On-site</strong></td>
			<td class="py-3">€900</td>
			<td class="py-3">800</td>
		</tr>
	</tbody>
</table>

For member rates, you must be a member of [ACM](https://acm.org "The Association for Computing Machinery") and/or [SIGCHI](https://sigchi.org " ACM Special Interest Group on Computer-Human Interaction"). You will be required to register using the same email address as your ACM account.

The advertised student rates are restricted to registered and currently active students only, you may be asked to provide evidence of your student status. If you cannot provide proof of student status, you will be required to register as a _professional_ attendee.

Workshops and the doctoral consortium are €80 each and must be registered for using ths registration system. If you have already registered, you can update your registration. You will not be able to attend a workshop or the doctoral consortium without registering for it.

All registration fees above are inclusive of Value Added Tax (VAT), which is charged at 17%. The registration system shows prices excluding VAT.

### Reduced rate for economically developing countries

CUI is committed to increasing the accessibility and diversity of the conference series. Following a tradition established a number of years ago, CUI 2024 is offering discounted registration to individuals based [in economically developing countries]({{ '/attend/discounted-registration/' | relative_url }} "Reduced Rate Eligibility for CUI {{ site.conference.year }}").

If eligible for the discount, you will be provided with a discount code at the end of the registration process that should be pasted into the discount text field for the discount to be applied.

## Need support or have a question?

{% for group in site.data.oc %}
	{% for role in group[1]['roles'] %}
		{%- if role[0] == 'registration' %}
<p>If you need any support or have questions about the registration process, please contact the <a href="{{ role[1].email }}" title="Email address for the CUI {{ site.conference.year }} {{ role[1].label }}">CUI {{ site.conference.year }} {{ role[1].label }}</a>.</p>
		{% break %}
		{% endif %}
	{% endfor %}
{% endfor %}