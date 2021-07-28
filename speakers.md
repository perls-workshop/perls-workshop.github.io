---
layout: default
---

# Plenary Speakers

<div class="row justify-content-center">
    {% for speaker in site.data.speakers %}
        {% if speaker.plenary %}
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
        {% endif %}
    {% endfor %}
</div>

# Confirmed Panelists

<div class="row justify-content-center">
    {% for panelist in site.data.speakers %}
        {% if panelist.panel %}
        {% unless panelist.keynote %}
        <div class="text-center speaker">
            <img src="{{ panelist.image }}" class="speaker-img" />

            <div class="break"></div>

            {% if panelist.website %}
            <a href="{{ panelist.website }}" target="_blank" >
                {{ panelist.name }}
            </a>
            {% else %}
                {{ panelist.name }}
            {% endif %}

            <div class="break"></div>

            <div class="speaker-affiliation">
            {% if panelist.affiliation %}
                {{ panelist.affiliation }}
            {% endif %}
            </div>
        </div>
        {% endunless %}
        {% endif %}
    {% endfor %}
</div>

