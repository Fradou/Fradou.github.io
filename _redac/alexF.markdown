---
title: Fnatic
layout: team
sname: FNC
---



Testons les formules :  

{% for expe in site.data.cv.experience %}
<h4>{{ expe.name }}</h4>
<p>{{expe.location }} - {{expe.start}} à {{expe.end}}</p>

{% for desc in expe.job_descr %}
* {{ desc.fonction}}
{% endfor %}
{% endfor %}
