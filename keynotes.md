---
layout: default
---
{% assign keynotes = site.data.keynote %}
{% assign speakers = keynotes.speakers %}

{% if speakers %}
# Keynote talks

{% for s in speakers %}

#### {{ s.speaker.courtesy_title }} {{ s.speaker.name }}, {{ s.speaker.affiliation }}, {{ s.speaker.country }} 

{% if s.speaker.photo %}
![{{ s.speaker.name }}]({{ s.speaker.photo }})
{% endif %}

{% if s.speaker.bio %}
**Bio**: {{ s.speaker.bio }}
{% endif %}

{% if s.speaker.title  %}
### {{ s.speaker.title }}
{% endif %}

{% if s.speaker.abstract %}
**Abstract**: {{ s.speaker.abstract }}
{% endif %}

---


{% endfor %}


{% else %}
The keynote talks have not been announced yet.
{% endif %}

