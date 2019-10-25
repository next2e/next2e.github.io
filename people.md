---
layout: main
---

# 2WebsitE - Residents and Friends

## RESIDENTS

---

{% for year in site.data.people.residents %}

### {{ year.year }}s

<div class="resident-bios">
  {% for person in year.people %}
  {% include bio.html year=year.year name=person.name kerberos=person.kerberos course=person.course description=person.description %}
  {% endfor %}
</div>

{% endfor %}

## ALUMS

---

{% for year in site.data.people.alums %}

### {{ year.year }}s

<div class="resident-bios">
  {% for person in year.people %}
  {% include bio.html year=year.year name=person.name kerberos=person.kerberos course=person.course description=person.description %}
  {% endfor %}
</div>
{% endfor %}

## FRIENDS

---

<div class="resident-bios">
  {% for person in site.data.people.friends %}
  {% include bio.html name=person.name kerberos=person.kerberos course=person.course description=person.description %}
  {% endfor %}
</div>

## KING GOURD

---

<div class="resident-bios">
  {% capture gourd_bio %}
  King Gourd humbly overlooked the masses of 2E, 2015-2015. He will be missed, though his portrait remains in his honor.
  {% endcapture %}
  {% include bio.html year="2015" name="King Gourd" kerberos="kgourd" course="23" description=gourd_bio %}
</div>