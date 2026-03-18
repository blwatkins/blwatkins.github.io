---
title: "home"
layout: base
---

# Brittni Watkins

Brittni is an educator, software developer, and algorithmic artist.
She is passionate about teaching people from all backgrounds how to code.
Her current research interests include algorithmic art, blockchain development, web application development, and DevSecOps.
The applications of computer programming are numerous and varied; there is space for everyone.

Brittni creates algorithmic art, photography, and music under her pseudonym, [**azurepolarbear**](https://azurepolarbear.github.io/).
You can purchase stationery and gifts featuring azurepolarbear's work from the [**brittni and the polar bear boutique**](https://brittniandthepolarbear.com/).

***There is beauty in code, and code can make beautiful things.***

## [portfolio](./portfolio.md)

## [learn to code](./learn-to-code)

----

# posts

{% assign posts = site.posts %}
{%- if posts.size > 0 -%}
  {%- if page.list_title -%}
  <h2 class="post-list-heading">{{ page.list_title }}</h2>
  {%- endif -%}
  <ul class="post-list">
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    {%- for post in posts -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      {%- if site.minima.show_excerpts -%}
      {{ post.excerpt }}
      {%- endif -%}
    </li>
    {%- endfor -%}
  </ul>
{%- endif -%}
