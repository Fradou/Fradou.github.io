---
layout: page
title: Recrutement
permalink: /recrutement/
---

Au délà de la passion pour League of Legends qui motive nos auteurs à produire un contenu de qualité, ce site est aussi un moyen de faire connaitre nos journalistes et freelancers.  
Notre travail vous plait ? Un des auteurs se démarque et vous souhaiteriez l'engager ?  

Voici la liste de nos auteurs actuellement ouvert aux propositions d'emploi :

{% for employ in site.data.curric %}
 {% assign emp = employ[1] %}
 {% if emp.seeking == "oui" %}
* {{ emp.name}}  
[CV]({{site.baseurl}}/curric/) - [Contact](mailto:{{emp.email}})
 {% else %}
* {{ emp.name}}
Ne souhaite pas être contacté pour le moment
{% endif %}
{% endfor %}


    
    
You can find the source code for the Jekyll new theme at:
{% include icon-github.html username="jglovier" %} /
[jekyll-new](https://github.com/jglovier/jekyll-new)

You can find the source code for Jekyll at
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)
