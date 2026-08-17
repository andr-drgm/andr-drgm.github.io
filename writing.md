---
layout: default
title: Writing
permalink: /writing/
description: Notes on scoping, deleting, and shipping software that earns its keep.
---

<section class="hero">
  <div class="wrap">
    <p class="eyebrow">Writing</p>
    <h1>Notes from the work.</h1>
    <p class="lede" style="margin-top:1.25rem;max-width:34rem">Scoping, deleting, and shipping software that earns its keep.</p>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <ul class="posts">
      {%- for post in site.posts %}
      <li>
        <a href="{{ post.url }}">
          <span class="meta">{{ post.date | date: "%b %Y" }}</span>
          <strong>{{ post.title }}</strong>
          {% if post.description %}<em>{{ post.description }}</em>{% endif %}
        </a>
      </li>
      {%- else %}
      <li><a href="/">Nothing published yet.</a></li>
      {%- endfor %}
    </ul>
  </div>
</section>
