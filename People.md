---
title: People
permalink: /People/
---

{% assign people_sorted = (site.people | sort: 'joined' %}
{% assign people_array = "pi|staff|postdoc|gradstudent|postbac|undergrad|highschool" | split: "|" %}

{% for item in people_array %}

<div class="pos_header">
{% if item == 'pi' %}
<h3>Principal Investigator</h3>
 {% elsif item == 'postdoc' %}
<h3>Postdoctoral Researchers</h3>
 {% elsif item == 'gradstudent' %}
<h3>Graduate Students</h3>
 {% elsif item == 'postbac' %}
<h3>Postbaccalaureate Researchers</h3>
 {% elsif item == 'visiting' %}
<h3>Visiting Researchers</h3>
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

<h5>Postdocs</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Yinan Dong | Postdoc | CSHL | 2023-2023 | Research Scientist at Meta |
Antonio Majdandzic | Postdoc | CSHL | 2020-2022 | ML Researcher at Bloomberg |
Rohit Tripathy | Postdoc | CSHL | 2020-2022 | Staff Scientist at Jackson Laboratory |

<h5>Undergrads</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Nika Chuzhoy | Undergrad Researcher | CalTech, Computer Science | Summer 2023 | |
Tianhao Luo | Summer Undergrad Research Program | UPenn, Statistics | Summer 2023 | |
Phillip Zhou | Summer Undergrad Research Program  | Amherst College, Math | Summer 2022 | |
Vandana Agarwala | Summer Undergrad Research Program | Penn State, Computer Science | Summer 2021 | Software developer at Flagship Pioneering |
Roshan Kenia | Undergrad Researcher | Stony Brook, Computer Science | 2020-2021 | Computer Science Masters Program at Columbia |

<h5>High Schoolers</h5>
 
| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Steven Yu | High School Researcher  | Syosset High | 2022-2023 | Undergrad at Columbia |
Amanda Nemshin | High School Researcher  | Cold Spring Harbor High | 2022-2023 | Undergrad at Duke |
Rohan Ghotra | High School Researcher  | Syosset High | 2021-2022 | Undergrad at Columbia |
Ethan Labelson | High School Researcher  | Friends Academy | 2021-2022 | Undergrad at Caltech |
Ashwin Narayanan | High School Researcher  | Jericho High | Summer 2022 | Undergrad at Johns Hopkins |
Zaara Yakub | High School Researcher | Bethpage High School | 2020-2021 | Undergrad at Lehigh |


<h5>Visiting researchers</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Eduardo Esteva | Masters Student | NYU, Bioinformatics | 2020-2021 | Bioinformatics Analyst at NYU Grossman School of Medicine |

<h5>Rotation Students</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Maha Sayed | Rotation Student | CSHL SBS | Spring 2023 | Grad student in Meyer Lab |
June He | Rotation Student | Stony Brook Genetics PhD student | Spring 2023 |  |
Lucia Tellez Perez | Rotation Student | CSHL SBS | Spring 2022 | Grad student in dos Santos Lab |
Thomas Huffstutler | Rotation Student | Stony Brook Applied Math Masters student | Spring 2022 | |
Joon-Hyun Song | Rotation Student | Stony Brook Applied Math PhD student | Winter 2021 | |
Scott Feltman | Rotation Student | Stony Brook Applied Math PhD student | Winter 2021 | |
Brenda Delamonica | Rotation Student | Stony Brook Applied Math Masters student | Fall 2021 | |
Sam Kleeman | Rotation Student | CSHL SBS | Spring 2021 | Grad student in Janowitz and Furukawa Labs |

<br>
<br>
<br>


