---
layout: page
title: Aktuelles
permalink: /aktuelles/
---

## Neuigkeiten aus dem Verein

{% for post in site.posts %}
  <article class="post">
    <h3>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
    <p class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">
        {{ post.date | date: "%b %-d, %Y" }}
      </time>
    </p>
    <div class="post-content">
      {{ post.excerpt }}
      <a href="{{ post.url | relative_url }}">Weiterlesen</a>
    </div>
  </article>
{% endfor %}
