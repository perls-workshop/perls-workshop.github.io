---
layout: default
---

<!-- Locate keynote speakers and panelists -->
{% assign num_keynotes = 0 %}
{% for speaker in site.data.speakers %}
  {% if speaker.keynote %}
    {% if num_keynotes == 0 %}{% assign keynote1 = speaker %}
    {% elsif num_keynotes == 1 %}{% assign keynote2 = speaker %}
    {% elsif num_keynotes == 2 %}{% assign keynote3 = speaker %}
    {% elsif num_keynotes == 3 %}{% assign keynote4 = speaker %}
    {% endif %}
    {% assign num_keynotes = num_keynotes | plus: 1 %}
  {% endif %}
{% endfor %}
{% assign panelists = site.data.speakers | sort: "panel" %}

# Workshop Draft Schedule

All details subject to change at this point.

## Workshop Day 1 (Monday, December 13th)

<table class="table schedule table-bordered table-hover">
<caption>Workshop draft schedule - Monday, December 13th</caption>
  <thead class="thead-light">
    <tr>
      <th scope="col" class="col-2">Time (EST)</th>
      <th scope="col" class="col-10" colspan="2">Event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">8:00am</th>
      <td colspan="2">Welcome</td>
    </tr>
    <tr>
      <th scope="row">8:05am</th>
      <td colspan="2">
        Keynote 1:
        {% if keynote1.website %}
          <a href="{{ keynote1.website }}" target="_blank" >
          {{ keynote1.name }}
          </a>
        {% else %}
          {{ keynote1.name }}
        {% endif %}
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">8:55am</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <!-- -->
    <tr class="theme-1">
      <th scope="row">9:00am</th>
      <td rowspan="2" class="col-1 theme-header">
        <p>Theme 1:</p>
        <p>Vagueness & Specification</p>
      </td>
      <td>
        Lightning talks & Panel discussion 1
        <ul>
        {% for speaker in panelists %}
          {% if speaker.panel == 'vs' %}
            <li>
              {% if speaker.website %}
                <a href="{{ speaker.website }}" target="_blank" >{{ speaker.name }}</a>
              {% else %}
                {{ speaker.name }}
              {% endif %}
            </li>
          {% endif %}
        {% endfor %}
        </ul>
      </td>
    </tr>
    <tr class="theme-1">
      <th scope="row">11:00am</th>
      <td>
        Poster session 1
        <ul>
          <li>Accepted Papers TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">12:00 Noon</th>
      <td colspan="2">Lunch break (1hr)</td>
    </tr>
    <!-- -->
    <tr class="theme-2">
      <th scope="row">1:00pm</th>
      <td rowspan="2" class="col-1 theme-header">
        <p>Theme 2:</p>
        <p>Trust & Power</p>
      </td>
      <td>
        Lightning talks & Panel discussion 2
        <ul>
        {% for speaker in panelists %}
          {% if speaker.panel == 'tp' %}
            <li>
              {% if speaker.website %}
                <a href="{{ speaker.website }}" target="_blank" >{{ speaker.name }}</a>
              {% else %}
                {{ speaker.name }}
              {% endif %}
            </li>
          {% endif %}
        {% endfor %}
        </ul>
      </td>
    </tr>
    <tr class="theme-2">
      <th scope="row">3:00pm</th>
      <td>
        Poster session 2
        <ul>
          <li>Accepted Papers TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">4:00pm</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <tr>
      <th scope="row">4:05pm</th>
      <td colspan="2">
        Keynote 2:
        {% if keynote2.website %}
          <a href="{{ keynote2.website }}" target="_blank" >
          {{ keynote2.name }}
          </a>
        {% else %}
          {{ keynote2.name }}
        {% endif %}
      </td>
    </tr>
    <tr>
      <th scope="row">4:55pm</th>
      <td colspan="2">Closing remarks</td>
    </tr>
  </tbody>
</table>

## Workshop Day 2 (Tuesday, December 14th)

<table class="table schedule table-bordered table-hover">
<caption>Workshop draft schedule - Tuesday, December 14th</caption>
  <thead class="thead-light">
    <tr>
      <th scope="col" class="col-2">Time (EST)</th>
      <th scope="col" class="col-10" colspan="2">Event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">8:00am</th>
      <td colspan="2">Welcome</td>
    </tr>
    <tr>
      <th scope="row">8:05am</th>
      <td colspan="2">
        Keynote 3:
        {% if keynote3.website %}
          <a href="{{ keynote3.website }}" target="_blank" >
          {{ keynote3.name }}
          </a>
        {% else %}
          {{ keynote3.name }}
        {% endif %}
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">8:55am</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <!-- -->
    <tr class="theme-3">
      <th scope="row">9:00am</th>
      <td rowspan="2" class="col-1 theme-header">
        <p>Theme 3:</p>
        <p>Multi-Agency</p>
      </td>
      <td>
        Lightning talks & Panel discussion 3
        <ul>
        {% for speaker in panelists %}
          {% if speaker.panel == 'ma' %}
            <li>
              {% if speaker.website %}
                <a href="{{ speaker.website }}" target="_blank" >{{ speaker.name }}</a>
              {% else %}
                {{ speaker.name }}
              {% endif %}
            </li>
          {% endif %}
        {% endfor %}
        </ul>
      </td>
    </tr>
    <tr class="theme-3">
      <th scope="row">11:00am</th>
      <td>
        Poster session 3
        <ul>
          <li>Accepted Papers TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">12:00 Noon</th>
      <td colspan="2">Lunch break (1hr)</td>
    </tr>
    <!-- -->
    <tr class="theme-4">
      <th scope="row">1:00pm</th>
      <td rowspan="2" class="col-1 theme-header">
        <p>Theme 4:</p>
        <p>Systems & Monopolization</p>
      </td>
      <td>
        Lightning talks & Panel discussion 4
        <ul>
        {% for speaker in panelists %}
          {% if speaker.panel == 'sm' %}
            <li>
              {% if speaker.website %}
                <a href="{{ speaker.website }}" target="_blank" >{{ speaker.name }}</a>
              {% else %}
                {{ speaker.name }}
              {% endif %}
            </li>
          {% endif %}
        {% endfor %}
        </ul>
      </td>
    </tr>
    <tr class="theme-4">
      <th scope="row">3:00pm</th>
      <td>
        Poster session 4
        <ul>
          <li>Accepted Papers TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">4:00pm</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <tr>
      <th scope="row">4:05pm</th>
      <td colspan="2">
        Keynote 4:
        {% if keynote4.website %}
          <a href="{{ keynote4.website }}" target="_blank" >
          {{ keynote4.name }}
          </a>
        {% else %}
          {{ keynote4.name }}
        {% endif %}
      </td>
    </tr>
    <tr>
      <th scope="row">4:55pm</th>
      <td colspan="2">Closing remarks</td>
    </tr>
  </tbody>
</table>


