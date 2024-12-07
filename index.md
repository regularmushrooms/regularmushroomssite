---
layout: home
title: "Regular Mushrooms"
---
<div class="container">

<h1> Welcome to Regular Mushrooms </h1>

</div>

<div class="container">

<h2> Explore our featured products: </h2>

{% assign mushroom_pages = site.pages | where: "categories", "Mushrooms" %}
    <ul class="my_list">
    {% for page in mushroom_pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endfor %}
    </ul>
</div>