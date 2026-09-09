---
layout: default
title: Home
---

<section class="masthead">
  <p class="kicker">A PERSONAL NOTEBOOK</p>
  <h1>{{ site.title }}</h1>
  <p class="subtitle">Ideas on science, mathematics, computing, and everything worth thinking about.</p>
</section>

<div class="rule"></div>

<section class="post-list">
{% for post in site.posts %}
  <article class="post-preview">
    <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | normalize_whitespace }}</p>
    <a class="read-more" href="{{ post.url | relative_url }}">Read the article →</a>
  </article>
{% endfor %}
</section>
