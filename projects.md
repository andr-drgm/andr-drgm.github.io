---
layout: default
title: Projects
permalink: /projects/
description: Case studies, projects and experience. Andrei Dragomir, software engineer.
---

<section>
  <div class="wrap">
    <div class="page-head">
      <p class="label">Case studies</p>
      <h2>What I've built</h2>
      <p>Live links and repos where they exist. Every name goes to the full write-up.</p>
    </div>
    <ul class="rows rows--media">
      {%- for post in site.posts %}
        {% include project-row.html post=post %}
      {%- endfor %}
    </ul>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Stack</p>
      <h2>What I reach for</h2>
    </div>
    <dl class="details">
      <dt>Backend &amp; data</dt>
      <dd>Ruby on Rails, Django, Node.js, Python, Ruby, PostgreSQL, Firebase, Supabase</dd>
      <dt>Frontend &amp; mobile</dt>
      <dd>TypeScript, React, Next.js, React Native, TailwindCSS, Kotlin</dd>
      <dt>Infra &amp; Web3</dt>
      <dd>Docker, CI/CD, Git, Puppeteer, Stripe, Solana, Solidity</dd>
    </dl>
  </div>
</section>
