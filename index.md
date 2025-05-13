---
title: 'home'
layout: home
---

# brittni | coding nerd

Brittni is an educator, software developer, and algorithmic artist.
She is passionate about teaching people from all backgrounds how to code.
Her current research interests include algorithmic art, blockchain development, web application development,
and DevSecOps. The applications of computer programming are numerous and varied; there is space for everyone.

Brittni creates algorithmic art, photography, and music under her pseudonym, [**azurepolarbear**](https://azurepolarbear.github.io/).
You can purchase stationery and gifts featuring azurepolarbear's work in the [brittni and the polar bear | code + art boutique](https://brittniandthepolarbear.com/).

***There is beauty in code, and code can make beautiful things.***

----

## latest post

<ul class="post-list">
{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
{% for post in site.posts limit:1 %}
  <li>
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  </li>
{% endfor %}
</ul>

----

## donate

We are currently accepting donations to support our creative projects.

<div>
  <p>
    <a href="https://www.buymeacoffee.com/brittniandthepolarbear"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=brittniandthepolarbear&button_colour=8828dc&font_colour=ffffff&font_family=Inter&outline_colour=ffffff&coffee_colour=FFDD00" /></a>
  </p>

  <p>
    <script type='text/javascript' src='https://storage.ko-fi.com/cdn/widget/Widget_2.js'></script><script type='text/javascript'>kofiwidget2.init('Support me on Ko-fi', '8828dc', 'O5O717Q6YA');kofiwidget2.draw();</script>
  </p>
<br/>
</div>

----

## All Posts
