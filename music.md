---
layout: page
title: Musique
permalink: /music/
---

### De la musique ? Qu'est ce que ça a à voir avec LoL ?

La plupart d'entre vous vont cliquer cet onglet de manière interrogative "Qu'est ce que ça a à voir avec LoL ? Pourquoi ils mettent ça ?" et j'en passe.  
Que vous y fassiez attention ou non, la musique et plus généralement les sons font partie de League of Legends et contribuent pour beaucoup à créer l'ambiance et le plaisir au sein du jeu (sauf pour ceux qui jouent sans son, bien entendu, mais dans ce cas vous manquez des trucs !!!).  
De manière générale, que ce soit un jeu vidéo, une série ou un film, la musique est souvent un facteur important mais discret pour dans la création d'univers, d'environnement, de situation.  

### Bon ok, et après ?

Etant tous des amateurs de musique, nous avons souhaité partagé entre nous, puis avec nos lecteurs, nos coup de coeurs et grandes musiques que ce soit jeu, série ou film.

Voici donc la playlist : 

{% for playlist in site.data.playlists %}
{% assign play = playlist[1] %}
**Selection de {{play.name}}**  
{% if play.comment %} {{play.comment}} {% endif %}
 {% for track in play.tracks %}
{{track.track}} - {{track.artist}}  
Se trouve dans {{track.origin}} - [link]({{track.link}})
{% endfor %}
{% endfor %}



