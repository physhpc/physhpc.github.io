---
layout: default
---
{% assign keynotes = site.data.keynote %}
{% assign speakers = keynotes.speakers %}

{% if speakers %}
# Keynote talks

{% for s in speakers %}

## Speaker

{% if s.speaker.photo %}
![{{ s.speaker.name }}]({{ s.speaker.photo }})
{% endif %}

### {{ s.speaker.courtesy_title }} {{ s.speaker.name }}, {{ s.speaker.affiliation }}, {{ s.speaker.country }} 
{{ s.speaker.bio }}

{% if s.speaker.title and s.speaker.abstract %}
### {{ s.speaker.title }}

{{ s.speaker.abstract }}


{% endif %}

---


{% endfor %}


{% else %}
The keynote talks have not been announced yet.
{% endif %}

