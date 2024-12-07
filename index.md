---
layout: default
title: "Regular Mushrooms"
---
<div class="container">

<h1> Welcome to Regular Mushrooms </h1>

</div>

<div class="container">

<h2> Explore our featured products: </h2>

{% assign mushroom_pages = site.pages | where: "categories", "Products" %}
    <ul class="my_list">
    {% for page in mushroom_pages %}
    <!-- <div class="container"> -->
        <li>
            <a href="{{ page.url }}"><img src="{{ page.link_image_path}}" alt="{{ page.link_image_name }}" style="width:160px; height:80px"></a>
            <p><a href="{{ page.url }}"> {{ page.title }} </a></p>
        </li>
    <!-- </div> -->
    {% endfor %}
    </ul>
</div>
