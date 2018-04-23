---
layout: post
title: My prueba de un post
summary: Esta es una prueba de como hacer un post y este texto es el resumen.
featured-img: nikon-d700-pictures
description: PRuebaaa meta description aaaassa sa dasd asd
categories: Category1, Category2
tags: [Test, Try, Prueba]
redirect_from:
  - prueba-redirect
---


## Prueba de h2

Esto imagino que sera un parrafo o algo asi



### Categorias de este post: 
<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.url}}/categorias/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>

#### Otra forma sin link
{{page.categories | capitalize | join: ', '}}

