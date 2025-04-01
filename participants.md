---
layout: page
title: Participants
participants:
  - {name: Philippe Cara, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Ilaria Colazzo, affiliation: "University of Leeds, United Kingdom"}
  - {name: Jan De Beule, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Bettina Eick, affiliation: "Technische Universität Braunschweig, Germany"}
  - {name: Leandro Vendramin, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Michel Lavrauw, affiliation: "University of Primorska, Slovenia"}
  - {name: Henrik Schanze, affiliation: "Technische Universität Braunschweig, Germany"}
  - {name: Max Horn, affiliation: "RPTU Kaiserslautern-Landau, Germany"}
  - {name: Leonard Soicher, affiliation: "Queen Mary University of London, United Kingdom"}
  - {name: Robin Simoens, affiliation: "Ghent University, Belgium and Universitat Politècnica de Catalunya, Spain"}
  - {name: Vinay Vilas Wagh, affiliation: "Indian Institute of Technology Guwahati, India"}
  - {name: Thomas Breuer, affiliation: "RWTH Aachen, Germany"}
  - {name: Meike Weiß, affiliation: "RWTH Aachen, Germany"}
  - {name: Ruth Hoffmann, affiliation: "University of St Andrews, Scotland"}
  - {name: Ahmed Khammash, affiliation: "Umm al-Qura University, Saudi Arabia"}
  - {name: Kamil Zabielski, affiliation: "Bialystok University of Technology, Poland"}
  - {name: Nour Alnajjarine, affiliation: "University of Rijeka, Croatia"}
  - {name: Tobias Ocula, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Rasmus Hvass Hansen, affiliation: "Danish Research Centre for Magnetic Resonance (DRCMR), Danmark"}
  - {name: Pavol Kollár, affiliation: "Comenius University in Bratislava, Slovakia"}
  - {name: Pieter-Jan Meuris, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Óscar Fernández Ayala, affiliation: "Technische Universität Braunschweig, Germany"}
  - {name: Janis Gathot, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Tudor Micu, affiliation: "Babeș-Bolyai University, Cluj-Napoca, Romania"}
  - {name: Karmele Garatea Zaballa, affiliation: "UPV/EHU, Spain"}
  - {name: Lukas Schnelle, affiliation: "RWTH Aachen, Germany"}
  - {name: Francesca Cavalieri, affiliation: "University of Padova, Italy"}
  - {name: Seyyed Ali Mohammadiyeh, affiliation: "Department of Pure Mathematics, Faculty of Mathematical Sciences, University of Kashan, Iran"}
  - {name: Sam Tertooy, affiliation: "KU Leuven, Kulak Kortrijk Campus, Belgium"}
  - {name: István Szöllősi, affiliation: "Babeș-Bolyai University, Cluj-Napoca, Romania"}
  - {name: Réka András, affiliation: "Robert Bosch SRL, Cluj-Napoca, Romania"}
  - {name: Mevlüde Alizade, affiliation: "Ankara University, Turkey"}
  - {name: Lara Deraedt, affiliation: "Ghent University, Belgium"}
  - {name: Rhys Evans, affiliation: "IMFM, Slovenia"}
  - {name: Jim Wittebol, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Kevin Piterman, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Maxime Deryck, affiliation: "Ghent University, Belgium"}
  - {name: Lander Meyts, affiliation: "Ghent University, Belgium"}
  - {name: Krisztián Nagy, affiliation: "Bolyai Institute University of Szeged, Hungary"}
  - {name: Rafał Lutowski, affiliation: "University of Gdańsk, Poland"}
  - {name: Michael Young, affiliation: "University of St Andrews, Scotland"}
  - {name: Komma Patali, affiliation: "Technische Universität Braunschweig, Germany"}
  - {name: Arne Van Antwerpen, affiliation: "Ghent University, Belgium"}
  - {name: Joe Edwards, affiliation: "University of St Andrews, Scotland"}
  - {name: Kobe Bleuzé, affiliation: "Ghent University, Belgium"}
  - {name: Charlotte Roelants, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Boris Fransen, affiliation: "University of Antwerp, Belgium"}
  - {name: Peter Birkner, affiliation: "Saarland University of Applied Sciences, Germany"}
  - {name: Thomas Deneve, affiliation: "Ghent University, Belgium"}
  - {name: Joseph Ward, affiliation: "University of St Andrews, Scotland"}
  - {name: Sarah Aoudia, affiliation: "University of St Andrews, Scotland"}
  - {name: Mun See Chang, affiliation: "University of St Andrews, Scotland"}
  - {name: Silvia Properzi, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Reinis Cirpons, affiliation: "University of St Andrews, Scotland"}
  - {name: Heleen Broodcoorens, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Leen Demuys, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Magdalena Wiertel, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Davide Ferri, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Andrew Darlington, affiliation: "Vrije Universiteit Brussel, Belgium"}
  - {name: Jozefien D'haeseleer, affiliation: "Ghent University, Belgium"}
  - {name: Manuel Delgado, affiliation: "University of Porto, Portugal"}
  - {name: James Mitchell, affiliation: "University of St Andrews, Scotland"}
  - {name: Russ Woodroofe, affiliation: "University of Primorska, Slovenia"}
  - {name: Guillaume Yziquel, affiliation: "VIZYON FRANCE (Grenbole), France"}
  - {name: Daimy Van Caudenberg, affiliation: "KU Leuven, Belgium"}
  - {name: Vlad Taranchuk, affiliation: "Ghent University, Belgium"}
  - {name: Milan Morreel, affiliation: "Ghent University, Belgium"}
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
