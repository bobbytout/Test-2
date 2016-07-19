---
layout: post
title:  "This is a test!"
date:   2016-07-16 11:07:58 +0200
categories: jekyll update
author: Fradou
---

Alors maintenant voyons ce que ça donne.

Déjà je voudrais voir si le page title : {{page.title}} marche ou si j'ai fumé.
Si je comprend bien, ça c'était un object.

Si je veux faire un tag, ça devrait être : {% if page.surname %}{{page.title}}{% elsif page.blabla %}{{"Désolé tu t'es chié bro"}}{%else%} {{site.title}}{% endif %}.

Et alors le filtre, comment ça marche je ne sais pas, donc testins là encore :
si je met : {{ "test" | site.title | page.title}} ça me donne quoi ?.

Et bingo on est parti pour voir ce que ça donne tout ça.
 
 
 Testons maintenant les data.
 Si je veux juste yellow, est ce que ça marche : 
 1 - {{data.Team.FNC.players[3].pseudo}}
 2 - {{Team.FNC.players[3]pseudo}}
 3 - {{Team.FNC.players.pseudo}}
 
 <ul>
{% for blob in site.data.Team %}
{% assign team = blob[1] %}
  <li>
    {{ team.org.shname }}
    {{ team.players | where:"spos","ADC" }}
    {{ team.players[pseudo] }}
    {{ team.players | size }} members
  </li>

{% endfor %}
</ul>


<ul>
{% for blob in site.data.Teams %}
  <li>
      {{ blob.adc }}
      {{ blob.name }}
    </a>
  </li>
{% endfor %}
</ul>

Et now on veux tester le plugin SoundClound :

soundcloud playlists 201483549

