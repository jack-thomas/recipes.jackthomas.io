---
layout: page
title: All Recipes
permalink: /all/
---

<div class="home">

  {%- assign posts = site.recipes | sort: 'title' -%}
  
  <ul class="post-list">
    {%- for post in posts -%}

    {%- assign categories = site.emptyArray -%}
    {%- for category in post.categories -%}
      {%- for subcategory in category["category"][0] -%}
        {%- assign categories = categories | push: subcategory -%}
      {%- endfor -%}
    {%- endfor -%}

    <li>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
    </li>
    {%- endfor -%}
  </ul>
</div>
