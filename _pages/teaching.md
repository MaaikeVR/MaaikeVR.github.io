---
layout: page
permalink: /teaching/
title: teaching
---

### Teaching Assistant 
I am / was a teaching assistant for the following courses:

{% for item in site.teaching %}
  <div style="text-indent: 2em;">
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

### Thesis Advisor

I am / was a daily advisor for the following master thesis students:

{% for item in site.master_thesis %}
  <div style="text-indent: 2em; padding-left: 0em;"> 
    <em>{{item.period}}</em>:
    {{item.name}},
    "{{item.title}}" <br/>
    <br/>
  </div>
{% endfor %}

<br />


### Ombuds Master Computer Science

I am the ombuds for both the Dutch Master Computerwetenschappen and the English Master in Computer Science at KU Leuven. You can reach me at <a href="mailto:ombuds-master-cs@kuleuven.be">ombuds-master-cs@kuleuven.be</a>.

<!-- 
{% if site.data.teaching.seminars and site.data.teaching.seminars.size>0 %}
    <h3> Seminars </h3>


    {% for item in site.data.teaching.seminars %}
        <div>
            <em>{{ item.date }}</em>:
            <strong> {{item.title}} </strong>
             <p>
                 @<a href="{{item.venue_url}}">{{item.venue}}</a>

                 {% if item.description %}<br>
                     {{ item.description }}
                 {% endif %}
             </p> 
        </div>
    {% endfor %}
{% endif %}
 -->

