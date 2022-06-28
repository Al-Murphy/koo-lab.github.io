---
title: People
permalink: /People/
---

{% assign people_sorted = (site.people | sort: 'joined' %}
{% assign people_array = "pi|staff|postdoc|gradstudent|rotation|visiting" | split: "|" %}

{% for item in people_array %}

<div class="pos_header">
{% if item == 'pi' %}
<h3>Principal Investigator</h3>
 {% elsif item == 'postdoc' %}
<h3>Postdoctoral Fellows</h3>
 {% elsif item == 'gradstudent' %}
<h3>Graduate Students</h3>
 {% elsif item == 'rotation' %}
<h3>Rotation Students</h3>
{% elsif item == 'undergrad' %}
<h3>Undergrad Researchers</h3>
{% elsif item == 'visiting' %}
<h3>High School Researchers</h3>
{% endif %}
</div>

<div class="content list people">
  {% for profile in people_sorted %}
    {% if profile.position contains item %}
    <div class="list-item-people">
      <p class="list-post-title">
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
        <a class="name" href="{{ site.baseurl }}{{ profile.url }}">{{ profile.name }}</a>
      </p>
    </div>    
    {% endif %}
  {% endfor %}
</div>
<hr>
{% endfor %}


<h3>Alumni</h3>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Lucia Tellez Perez | Rotation Student | CSHL SBS | Spring 2022 |  |
Thomas Huffstutler | Rotation Student | Stony Brook Applied Math Masters student | Spring 2022 | |
Vandana Agarwala | Summer Undergrad Research Program | Penn State, Computer Science | Summer 2021 | |
Brenda Delamonica | Rotation Student | Stony Brook Applied Math Masters student | Fall 2021 | |
Sam Kleeman | Rotation Student | CSHL SBS | Spring 2021 | Grad student in Janowitz and Furukawa Labs |
Roshan Kenia | Undergrad Researcher | Stony Brook, Computer Science | 2020-2021 | Intern at SupplyHouse.com |
Eduardo Esteva | Masters Student | NYU, Bioinformatics | 2020-2021 | Bioinformatics Analyst at NYU Grossman School of Medicine, Office of Science & Research|
Zaara Yakub | High School Researcher | Partners for the Future Program, Bethpage High School | 2020-2021 | Undergrad at Lehigh University |

<br>
<br>
<br>


