---
layout: page
permalink: /teaching/
title: teaching
# description: I am a teaching assistant for the following courses
---

### Teaching Assistant 
<!-- I am a teaching assistant for the following courses:   -->

{% for item in site.teaching %}
  <div style="text-indent: 0em;">
    <em>{{ item.period }}</em>:
    <strong>
        {{ item.course }}
    </strong>

    {% if item.note %}
      <p>
        {{ item.note }}
      </p>
    {% endif %}
    <br/> <br/>
  </div>
{% endfor %}  
  
<br />

<!-- I am a daily advisor for the following master thesis students:   -->

### Thesis Advisor

{% for item in site.master_thesis %}
  <div style="text-indent: -1em; padding-left: 1em;"> 
    <em>{{item.period}}</em>:
    {{item.name}},
    "{{item.title}}" <br/>
    <br/>
  </div>
{% endfor %}

<br />


### Ombuds Master Computer Science

I am the ombuds for both the Dutch Master Computerwetenschappen and the English Master in Computer Science at KU Leuven. You can reach me at <a href="mailto:ombuds-master-cs@kuleuven.be">ombuds-master-cs@kuleuven.be</a>.
