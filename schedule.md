---
layout: default
---

<!-- Locate plenary speakers and panelists -->
{% for speaker in site.data.speakers %}
  {% if speaker.plenary == 1 %}
    {% assign plenary1 = speaker %}
  {% elsif speaker.plenary == 2 %}
    {% assign plenary2 = speaker %}
  {% endif %}
{% endfor %}
{% assign panelists = site.data.speakers | sort: "panel" %}

# Workshop Draft Schedule (Monday, December 13th)

All details subject to change.

<table class="table schedule table-bordered table-hover">
<caption>Workshop draft schedule - Monday, December 13th</caption>
  <thead class="thead-light">
    <tr>
      <th scope="col" class="col-2">Time (<a href="https://www.timeanddate.com/time/zones/pt">PT</a>)</th>
      <th scope="col" class="col-10" colspan="2">Event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">8:00am</th>
      <td colspan="2">Welcome</td>
    </tr>
    <tr>
      <th scope="row">8:20am</th>
      <td colspan="2">
        Opening plenary:
        {% if plenary1.website %}
          <a href="{{ plenary1.website }}" target="_blank" >
          {{ plenary1.name }}
          </a>
        {% else %}
          {{ plenary1.name }}
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
      <td class="col-1 theme-header">
        <p>Theme 1:</p>
        <p>Vagueness & Specification</p>
      </td>
      <td>
        <span class="theme-summary-label">Theme Summary:</span>
        <span class="theme-summary">
          How should RL systems be designed in the face of difficult specification problems and normative indeterminacies?
          How do these problems change in particular domains or as RL systems become more capable?
        </span>
        <hr />
        Lightning talks & Panel discussion 1
        <ul>
          <li>Speakers and panellists TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">9:55am</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <!-- -->
    <tr class="theme-2">
      <th scope="row">10:00am</th>
      <td class="col-1 theme-header">
        <p>Theme 2:</p>
        <p>Legitimacy, Accountability,<br />
        & Feedback</p>
      </td>
      <td>
        <span class="theme-summary-label">Theme Summary:</span>
        <span class="theme-summary">
          To what extent does RL automate many feedback mechanisms for oversight and control that social institutions (e.g. governments) presently enforce or take for granted?
          How can stakeholders acquire a voice in system evaluation?
        </span>
        <hr />
        Lightning talks & Panel discussion 2
        <ul>
          <li>Speakers and panellists TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">12:00 Noon</th>
      <td colspan="2">Lunch break (1hr)</td>
    </tr>
    <!-- -->
    <tr class="">
      <th scope="row">1:00pm</th>
      <td colspan="2">
        Poster session
        <ul>
          <li>Accepted Papers TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">2:55pm</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <!-- -->
    <tr class="theme-3">
      <th scope="row">3:00pm</th>
      <td class="col-1 theme-header">
        <p>Theme 3:</p>
        <p>Tools for democratization</p>
      </td>
      <td>
        <span class="theme-summary-label">Theme Summary:</span>
        <span class="theme-summary">
          What new policy tools (technical or otherwise) could be used to achieve democratic control and oversight of RL systems?
          What organizational theories are needed to inform or shape how democratization should proceed?
        </span>
        <hr />
        Lightning talks & Panel discussion 3
        <ul>
          <li>Speakers and panellists TBA</li>
        </ul>
      </td>
    </tr>
    <!-- -->
    <tr class="table-secondary">
      <th scope="row">4:55pm</th>
      <td colspan="2">Short break (5m)</td>
    </tr>
    <tr>
      <th scope="row">5:00pm</th>
      <td colspan="2">
        Closing plenary:
        {% if plenary2.website %}
          <a href="{{ plenary2.website }}" target="_blank" >
          {{ plenary2.name }}
          </a>
        {% else %}
          {{ plenary2.name }}
        {% endif %}
      </td>
    </tr>
  </tbody>
</table>
