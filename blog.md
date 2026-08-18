---
layout: default
title: Blog
permalink: /blog/
description: Notes on scoping, deleting, and shipping software that earns its keep.
---

<section>
  <div class="wrap">
    <div class="page-head">
      <h1>Notes from the work.</h1>
      <p class="lede">Scoping, deleting, and shipping software that earns its keep.</p>
    </div>
    <ul class="rows">
      {%- for post in site.posts %}
      <li>
        <div>
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <span class="meta">{{ post.date | date: "%d %B %Y" }}</span>
        </div>
        <div class="row-body">
          {% if post.description %}<p>{{ post.description }}</p>{% endif %}
        </div>
      </li>
      {%- else %}
      <li><p>Nothing published yet.</p></li>
      {%- endfor %}
    </ul>
  </div>
</section>
