---
title: "home"
layout: base
---

# brittni - coding nerd

Brittni is an educator, software developer, and algorithmic artist.
She is passionate about teaching people from all backgrounds how to code.
Her current research interests include algorithmic art, blockchain development, web application development, and DevSecOps.
The applications of computer programming are numerous and varied; there is space for everyone.

Brittni creates algorithmic art, photography, and music under her pseudonym, [**azurepolarbear**](https://azurepolarbear.github.io/).
You can purchase stationery and gifts featuring azurepolarbear's work from the [**brittni and the polar bear boutique**](https://brittniandthepolarbear.com/).

***There is beauty in code, and code can make beautiful things.***

----

# [learn to code](./learn-to-code)

Development of our tutorials is ongoing.

- ## [unix](./learn-to-code/unix)
- ## [git](./learn-to-code/version-control/git)
  - ### [github](./learn-to-code/version-control/git/github)
- ## [programming](./learn-to-code/programming)
  - ### [html](./learn-to-code/programming/html)
  - ### [typescript](./learn-to-code/programming/typescript)
- ## code scanning
  - ### [codeql](./learn-to-code/tools/code-scanning/codeql)
- ## [algorithmic art](./learn-to-code/algorithmic-art)
- ## [cryptography](./learn-to-code/cryptography)
  - ### [asymmetric encryption](./learn-to-code/cryptography/asymmetric-encryption)
- ## [networks](./learn-to-code/networks)
- ## [resources](./learn-to-code/resources.md)

----

# donate

We are currently accepting donations to support the development of this site and other projects.

<div style="text-align: center">
  <p>
    <a href="https://www.buymeacoffee.com/brittniandthepolarbear"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=brittniandthepolarbear&button_colour=8828dc&font_colour=ffffff&font_family=Inter&outline_colour=ffffff&coffee_colour=FFDD00" /></a>
  </p>

  <p>
    <script type='text/javascript' src='https://storage.ko-fi.com/cdn/widget/Widget_2.js'></script><script type='text/javascript'>kofiwidget2.init('Support me on Ko-fi', '8828dc', 'O5O717Q6YA');kofiwidget2.draw();</script>
  </p>
</div>

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
