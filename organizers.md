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

# Workshop Programme Comittee

In addition to the workshop organizers, our workshop programme comitte includes the following members:
<a target="blank" href="https://research.qut.edu.au/adms/people/abdul-obeid/">Abdul Obeid</a>, 
<a target="blank" href="https://researchers.uq.edu.au/researcher/24776">Archie Chapman</a>, 
<a target="blank" href="https://www.linkedin.com/in/xiaoguo-neuhkuuq">Xiao Guo</a>, 
<a target="blank" href="https://au.linkedin.com/in/camerondgordon">Cameron Gordon</a>, 
<a target="blank" href="https://www.admscentre.org.au/henry-fraser/">Henry Fraser</a>, 
<a target="blank" href="http://tttor.github.io/">Vektor Dewanto</a>, 
<a target="blank" href="https://simons.berkeley.edu/people/daniela-cialfi">Daniela Cialfi</a>, 
<a target="blank" href="https://rohancalum.github.io/">Rohan Nuttall</a>, 
<a target="blank" href="https://cyber.harvard.edu/people/svandergraaf">Shenja van der Graaf</a>, 
<a target="blank" href="https://www.tudelft.nl/en/tpm/about-the-faculty/departments/engineering-systems-and-services/people/assistant-professors/drir-rij-roel-dobbe/">Roel Dobbe</a>, 
<a target="blank" href="https://www.natolambert.com/">Nathan Lambert</a>, 
<a target="blank" href="http://scholar.google.ca/citations?user=lmQmYPgAAAAJ">Alan Chan</a>, 
<a target="blank" href="https://people.eecs.berkeley.edu/~sarahdean/">Sarah Dean</a>, 
<a target="blank" href="https://apps.ualberta.ca/directory/person/peetpare">Garnet Liam Peet-Pare</a>, 
<a target="blank" href="http://jrwright.info/">James Wright</a>, 
<a target="blank" href="https://medium.com/@charlesyang_32909">Charles Yang</a>, 
<a target="blank" href="https://www.ischool.berkeley.edu/people/nick-merrill">Nick Merrill</a>, 
<a target="blank" href="https://www.vivianeclay.com/">Viviane Clay</a>, 
<a target="blank" href="https://www.lesswrong.com/users/nora_ammann">Nora Ammann</a>, 
<a target="blank" href="https://imkaidu.net/index.html">Kai (David) Du</a>, 
<a target="blank" href="https://future-students.uq.edu.au/stories/meet-muhammad-pakistan-studying-it-australia">Muhammad Salman Mushtaq</a>, 
<a target="blank" href="https://acems.org.au/our-people/jun-ju">Jun Ju</a>.

