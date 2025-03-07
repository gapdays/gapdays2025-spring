---
layout: page
title: Participants
participants:
  - {name: Philippe Cara, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Ilaria Colazzo, affiliation: "University of Leeds, United Kingdom"}
  - {name: Jan De Beule, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Bettina Eick, affiliation: "Technische Universität Braunschweig"}
  - {name: Leandro Vendramin, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Michel Lavrauw, affiliation: "University of Primorska, Slovenia"}
  - {name: Henrik Schanze, affiliation: "Technische Universität Braunschweig"}
  - {name: Max Horn, affiliation: "RPTU Kaiserslautern-Landau"}
  - {name: Leonard Soicher, affiliation: "Queen Mary University of London"}
  - {name: Robin Simoens, affiliation: "Ghent University and Universitat Politècnica de Catalunya"}
  - {name: Vinay Vilas Wagh, affiliation: "Indian Institute of Technology Guwahati, India (IIT Guwahati)"}
  - {name: Thomas Breuer, affiliation: "Lehrstuhl für Algebra und Zahlentheorie, RWTH Aachen"}
  - {name: Meike Weiß, affiliation: "RWTH Aachen"}
  - {name: Ruth Hoffmann, affiliation: "University of St Andrews"}
  - {name: Ahmed Khammash, affiliation: "UQU"}
  - {name: Kamil Zabielski, affiliation: "Bialystok University of Technology"}
  - {name: Nour Alnajjarine, affiliation: "University of Rijeka"}
  - {name: Tobias Ocula, affiliation: "Vrije Universiteit Brussel"}
  - {name: Rasmus Hvass Hansen, affiliation: "Danish Research Centre for Magnetic Resonance (DRCMR)"}
  - {name: Pavol Kollár, affiliation: "Comenius University in Bratislava, Slovakia"}
  - {name: Pieter-Jan Meuris, affiliation: "Vrije Universiteit Brussel"}
  - {name: Óscar Fernández Ayala, affiliation: "Technische Universität Braunschweig"}
  - {name: Janis Gathot, affiliation: "Vrije Universiteit Brussel"}
  - {name: Tudor Micu, affiliation: "Babeș-Bolyai University, Cluj-Napoca (Romania)"}
  - {name: Karmele Garatea Zaballa, affiliation: "UPV/EHU"}
  - {name: Lukas Schnelle, affiliation: "SLA/ART RWTH Aachen"}
  - {name: Francesca Cavalieri, affiliation: "University of Padova"}
  - {name: Seyyed Ali Mohammadiyeh, affiliation: "Department of Pure Mathematics, Faculty of Mathematical Sciences, University of Kashan, Kashan,Iran"}
  - {name: Pushpendra Singh, affiliation: "Indian Institute of Technology Jodhpur, India"}
  - {name: Sam Tertooy, affiliation: "KU Leuven, Kulak Kortrijk Campus"}
  - {name: István Szöllősi, affiliation: "Babeș-Bolyai University, Cluj-Napoca (Romania)"}
  - {name: Réka András, affiliation: "Robert Bosch SRL, Cluj-Napoca (Romania)"}
  - {name: Mevlüde Alizade, affiliation: "Ankara University"}
  - {name: Lara Deraedt, affiliation: "Ghent University"}
  - {name: Rhys Evans, affiliation: "IMFM"}
  - {name: Jim Wittebol, affiliation: "Vrije Universiteit Brussel"}
  - {name: Kevin Piterman, affiliation: "Vrije Universiteit Brussel"}
  - {name: Maxime Deryck, affiliation: "Ghent University"}
  - {name: Lander Meyts, affiliation: "Ghent University"}
  - {name: Krisztián Nagy, affiliation: "Bolyai Institute University of Szeged"}
  - {name: Rafał Lutowski, affiliation: "University of Gdańsk"}
  - {name: Michael Young, affiliation: "University of St Andrews"}
  - {name: Komma Patali, affiliation: "Technische Universität Braunschweig"}
  - {name: Arne Van Antwerpen, affiliation: "Ghent University"}
  - {name: Joe Edwards, affiliation: "University of St Andrews"}
  - {name: Kobe Bleuzé, affiliation: "Ghent University"}
  - {name: Charlotte Roelants, affiliation: "Vrije Universiteit Brussel"}
  - {name: Boris Fransen, affiliation: "University of Antwerp"}
  - {name: Peter Birkner, affiliation: "Saarland University of Applied Sciences"}

---

<ol>{% assign participants = page.participants | sort: "name" %}
{% for p in participants %}
  <li>
    <strong>{{ p.name }}</strong>
    {% if p.affiliation != null %} ({{ p.affiliation }}){% endif %}
    {% if p.links != null %}
        {% for item in p.links %}
            <a href="{{ item[1] }}">({{ item[0] }})</a>
        {% endfor %}
    {% endif %}
    <br/>
      {% if p.talk != null %} Talk: {{ p.talk }}{% endif %}
  </li>
{% endfor %}
</ol>

{% if site.data.feedback.size > 0 %}

<ul>
{% for p in site.data.feedback %}
  <li>
    <strong>{{ p.name }}</strong>
    {% if p.package != null %} (author of {{ p.package }}){% endif %}
    <br/>
    {% if p.feedback != null %} {{ p.feedback }}{% endif %}
  </li>
{% endfor %}
</ul>

{% endif %}

<!--
## Conference photo
[<img src="{{ site.baseurl }}/public/conf_photo.jpg" />]({{ site.baseurl }}/public/conf_photo.jpg)
-->
