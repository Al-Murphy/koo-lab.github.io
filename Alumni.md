---
title: Alumni
permalink: /Alumni/
---

{% assign people_sorted = (site.people | sort: 'joined' %}
{% assign people_array = "alumni" | split: "|" %}

{% for item in people_array %}

<div class="pos_header">
{% if item == 'alumni' %}
<h3>Alumni</h3>--->
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
