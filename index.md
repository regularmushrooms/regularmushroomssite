---
layout: default
title: "Regular Mushrooms"
paginate: true
---
<div class="container">

<h1> Welcome to Regular Mushrooms </h1>

</div>

<div class="container">
    <h2>Explore our Featured Products</h2>
    <div class="gallery">
        {% assign mushroom_pages = site.pages | where: "categories", "Products" %}
        {% for page in mushroom_pages %}
        <div class="gallery-item">
            <a href="{{ page.url }}">
                <img src="{{ page.link_image_path }}" alt="{{ page.link_image_name }}" class="gallery-image">
            </a>
            <p class="gallery-title"><a href="{{ page.url }}">{{ page.title }}</a></p>
        </div>
        {% endfor %}
    </div>
</div>

