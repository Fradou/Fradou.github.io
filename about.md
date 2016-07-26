---
layout: page
title: About
permalink: /about/
---

### Le site

League Of News est un tout nouveau site d'actualités destiné à la communauté francophone de League Of Legends. L'aventure démarre en juillet 2016 suite à un projet "examen" pour l'entrée en formation d'un de nos membres fondateurs.

Autour du site s'est au fur et à mesure regroupé une équipe de passionnés, chacun apportant son champs d'expertise, du challenger qui vous donne les protips au fanboy qui vous tiendra au courant des ragots et transfert dans les teams sans oublier le webdev qui s'occupe de faire tourner tout ça. 

### L'équipe

Au délà de la passion pour League of Legends qui reste le motivation première pour chacun d'entre nous, ce site est également un moyen pour nos auteurs et contributeurs, principalement des indépendants et freelances, de se faire connaître et démontrer leur talent dans leur domaine.  

Notre travail vous plait ? Le style ou profil d'un de nos membres vous interésse ?  

Vous trouverez ci-dessous la liste de notre équipe, leur occupation dans et hors du site ainsi que leur statut actuel :

{% for employ in site.data.curric %}
 {% assign emp = employ[1] %}
* {{ emp.name}} - {{emp.titlebl}} sur LeagueOfNews - {{emp.title}}  
 {% if emp.seeking == "oui" %}[CV]({{site.baseurl}}/redac/{{employ[0]}}.html) - [Contact](mailto:{{emp.email}})  
 {% else %}Ne souhaite pas être contacté pour le moment.
{% endif %}
{% endfor %}


Au cas où :

You can find the source code for the Jekyll new theme at:
{% include icon-github.html username="jglovier" %} /
[jekyll-new](https://github.com/jglovier/jekyll-new)

You can find the source code for Jekyll at
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)
