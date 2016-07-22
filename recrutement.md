---
layout: page
title: Recrutement
permalink: /recrutement/
---

Au délà de la passion pour League of Legends qui motive nos auteurs à produire un contenu de qualité, ce site est aussi un moyen de faire connaitre nos journalistes en herbes.  
Notre travail vous plait ? Un des auteurs se démarque et vous souhaiteriez l'engager ?  

Voici la liste de nos auteurs actuellement ouvert aux propositions d'emploi :

{% for employ in site.data.curric %}
 {% if employ[1].seeking == "oui" %}
 <ul>{{ employ[1].name}} [CV]({{site.baseurl}}/curric/)</ul>
{% endif %}
{% endfor %}


test 2

{% if site.data.curric.alexF.seeking == "oui" %}
 gg
 {% endif %}



Testons les formules :  

{% for expe in site.data.cv.experience %}
<h4>{{ expe.name }}</h4>
<p>{{expe.location }} - {{expe.start}} à {{expe.end}}</p>

{% for desc in expe.job_descr %}
* {{ desc.fonction}}
{% endfor %}
{% endfor %}
    
