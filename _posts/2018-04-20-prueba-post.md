---
layout: post
title: My prueba de un post
summary: Esta es una prueba de como hacer un post y este texto es el resumen.
featured-img: nikon-d700-pictures
description: PRuebaaa meta description aaaassa sa dasd asd
<<<<<<< HEAD
categories: [Category1, category2]
tags: [test, try, prueba]
=======
categories: Category1, Category2
tags: [Test, Try, Prueba]
redirect_from:
  - prueba-redirect
>>>>>>> 7b9996c9d47ce44914b653a25ed2a573cc07147c
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

