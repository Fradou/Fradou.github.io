---
layout: page
title: About
permalink: /about/
---

###Le site

League Of News est un tout nouveau site d'actualités destiné à la communauté francophone de League Of Legends.

Autour du site s'est regroupé une équipe de passionnés, chacun apportant son champs d'expertise, du challenger qui vous donne les protips au fanboy qui vous tiendra au courant des ragots et transfert dans les teams sans oublier le webdev qui s'occupe de faire tourner tout ça. 

Retrouvez nous sur les réseaux sociaux :
{% include icon-twitter.html username="LoL_of_News" %}

Au délà de la passion pour League of Legends qui reste le motivation première pour chacun d'entre nous, ce site est également un moyen pour nos auteurs et contributeurs, principalement des indépendants et freelances, de se faire connaître et démontrer leur talent dans leur domaine.  

Notre travail vous plait ? Un des auteurs se démarque et vous souhaiteriez l'engager ?  

Vous trouverez ci-dessous la liste de notre équipe, leur occupation dans et hors du site ainsi que leur statut actuel :

{% for employ in site.data.curric %}
 {% assign emp = employ[1] %}
* {{ emp.name}} - {{emp.titlebl}} sur LeagueOfNews - {{emp.title}}  
 {% if emp.seeking == "oui" %}[CV]({{site.baseurl}}/redac/{{employ[0]}}.html) - [Contact](mailto:{{emp.email}})  
 {% else %}Ne souhaite pas être contacté pour le moment.
{% endif %}
{% endfor %}
