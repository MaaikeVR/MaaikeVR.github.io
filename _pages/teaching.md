---
layout: page
permalink: /teaching/
title: teaching
# description: I am a teaching assistant for the following courses
---
I am a teaching assistant for the following courses:  

{% for item in site.teaching %}
  <div style="text-indent: 1em;">
    <em>{{ item.period }}</em>:
    <strong>
        {{ item.course }}
    </strong>

    {% if item.note %}
      <p>
        {{ item.note }}
      </p>
    {% endif %}
  </div>
{% endfor %}  
  
<br />

I am a daily advisor for the following master thesis students:  

{% for item in site.master_thesis %}
  <div style="text-indent: 1em;"> 
    <em>{{item.period}}</em>:
    {{item.name}},
    "{{item.title}}"
  </div>
{% endfor %}

