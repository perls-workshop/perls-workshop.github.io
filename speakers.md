---
layout: default
---

# Confirmed Speakers and Panellists

<div class="row justify-content-center">
    {% for speaker in site.data.speakers %}
    <div class="text-center speaker">
        <img src="{{ speaker.image }}" class="speaker-img" />

        <div class="break"></div>

        {% if speaker.website %}
        <a href="{{ speaker.website }}" target="_blank" >
            {{ speaker.name }}
        </a>
        {% else %}
            {{ speaker.name }}
        {% endif %}

        <div class="break"></div>

        <div class="speaker-affiliation">
        {% if speaker.affiliation %}
            {{ speaker.affiliation }}
        {% endif %}
        </div>
    </div>
    {% endfor %}
</div>
