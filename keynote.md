---
layout: default
---

# Keynote talks



{% assign keynotes = site.data.keynote %}
{% assign speakers = keynotes.speakers %}


{% for s in keynotes.speakers %}
## Speaker
### {{ s.speaker.courtesy_title }} {{ s.speaker.name }}, {{ s.speaker.affiliation }}, {{ s.speaker.country }} 
![imgSpeaker]({{ s.speaker.photo }})
{{ s.speaker.bio }}
### {{ s.speaker.title }}
{{ s.speaker.abstract }}
---
{% endfor %}
