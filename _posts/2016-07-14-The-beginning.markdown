---
layout: post
title:  "This is a test!"
date:   2016-07-14 11:07:58 +0200
---


First one yessssssssssss
Attentat à nice sadly.
Ca donne quoi ca : {% post_url 2016-07-17-This-s-a-test %}

Testons un peu les objects :
Est ce que je peux avoir les all-tags : 
{{blog.all_tags}}
Alors ?
Tous les articles maybes ?
{{blog.articles}}
Avec la boucle c'est mieux ?
{% for article in blog.articles %}
    <h2>{{ article.title }}</h2>
{% endfor %}

Combien j'ai darticles ? et bien : {{blog.articles_count}}
