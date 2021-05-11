---
layout: default
---

# Workshop Organizers

<div class="container">
    {% for organizer in site.data.organizers %}
    <div class="organizer row">
        <div class="col-md-auto text-center">
            <img src="{{ organizer.image }}" class="organizer-img" />
            <div class="break"></div>
            {% if organizer.website %}
            <a href="{{ organizer.website }}" target="_blank" >
                {{ organizer.name }}
            </a>
            {% else %}
                {{ organizer.name }}
            {% endif %}
        </div>

        <div class="organizer-bio col">{{ organizer.bio }}</div>
    </div>
    {% endfor %}
</div>

