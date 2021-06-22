---
layout: default
---

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
        {% for speaker in site.data.speakers | sort: "keynote" limit:1 offset:0 %}
          {% if speaker.website %}
            <a href="{{ speaker.website }}" target="_blank" >
            {{ speaker.name }}
            </a>
          {% else %}
            {{ speaker.name }}
          {% endif %}
        {% endfor %}
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
        {% for speaker in site.data.speakers | sort: "panel" %}
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
        {% for speaker in site.data.speakers | sort: "panel" %}
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
        {% for speaker in site.data.speakers | sort: "keynote" limit:1 offset:1 %}
          {% if speaker.website %}
            <a href="{{ speaker.website }}" target="_blank" >
            {{ speaker.name }}
            </a>
          {% else %}
            {{ speaker.name }}
          {% endif %}
        {% endfor %}
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
        {% for speaker in site.data.speakers | sort: "keynote" limit:1 offset:2 %}
          {% if speaker.website %}
            <a href="{{ speaker.website }}" target="_blank" >
            {{ speaker.name }}
            </a>
          {% else %}
            {{ speaker.name }}
          {% endif %}
        {% endfor %}
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
        {% for speaker in site.data.speakers | sort: "panel" %}
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
        {% for speaker in site.data.speakers | sort: "panel" %}
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
        {% for speaker in site.data.speakers | sort: "keynote" limit:1 offset:3 %}
          {% if speaker.website %}
            <a href="{{ speaker.website }}" target="_blank" >
            {{ speaker.name }}
            </a>
          {% else %}
            {{ speaker.name }}
          {% endif %}
        {% endfor %}
      </td>
    </tr>
    <tr>
      <th scope="row">4:55pm</th>
      <td colspan="2">Closing remarks</td>
    </tr>
  </tbody>
</table>


