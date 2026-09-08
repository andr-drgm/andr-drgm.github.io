---
layout: default
title: Home
description: Andrei Dragomir: working software and technical direction for founders and operations teams building internal platforms, automation and MVPs.
---

{%- comment -%}
First viewport is the splash: name, nav, socials, nothing else. Everything below it
is the about page, folded in — /about/ no longer exists as its own URL, so this copy
lives in exactly one place. The transition between the two is in main.css.
{%- endcomment -%}
<section class="splash">
  <div class="splash-main">
    <div class="brand brand-lg">
      <img src="/assets/img/andrei.jpg" alt="" width="128" height="128" decoding="async">
      {% include wordmark.html %}
    </div>
    <nav class="splash-nav">
      {%- include nav.html -%}
    </nav>
  </div>
  <div class="splash-foot">
    <a class="splash-cue" href="#about">scroll <span aria-hidden="true">↓</span></a>
    {% include socials.html %}
  </div>
</section>

<section id="about">
  <div class="wrap">
    <div class="about-head">
      <div>
        <h1>Working software, and someone to own the decisions behind it.</h1>
        <p class="lede" style="margin-top:1.25rem">I build internal platforms, automation systems and MVPs for founders and operations teams, and take on the technical direction that comes with them: what gets built, in what order, and what it will cost to live with later.</p>
      </div>
      <img class="portrait" src="/assets/img/andrei.jpg" alt="Andrei Dragomir" width="720" height="900" decoding="async">
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">How it helps</p>
      <h2>What you get out of it</h2>
    </div>
    <ol class="numbered">
      <li>
        <h3>One person accountable</h3>
        <p>You always know who made the technical call and why. No decisions left waiting for someone to claim them.</p>
      </li>
      <li>
        <h3>A plan before the first line of code</h3>
        <p>Scope, sequence, and the parts we're deliberately not building, agreed together before anything gets built.</p>
      </li>
      <li>
        <h3>Something real, in weeks</h3>
        <p>Working software in front of users early, not a demo that only survives the happy path.</p>
      </li>
      <li>
        <h3>Code that outlives the engagement</h3>
        <p>Written for whoever picks it up next, including the team you hire after me.</p>
      </li>
    </ol>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Selected work</p>
      <h2>Three I'm building right now</h2>
      <p>Each one is a case study: the problem, the decisions that shaped it, and what changed after it shipped.</p>
    </div>
    <ul class="rows rows--media">
      {%- for post in site.posts limit: 3 %}
        {% include project-row.html post=post %}
      {%- endfor %}
    </ul>
    <p class="section-foot"><a href="/projects/">All projects →</a></p>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">When to engage</p>
      <h2>Three moments I'm usually called in</h2>
    </div>
    <ul class="rows">
      <li>
        <div>
          <h3>The idea is validated, nothing exists yet</h3>
          <span class="stack">Founders · Early-stage startups</span>
        </div>
        <div class="row-body">
          <p>We agree on what has to be proven first, cut what doesn't serve it, and put a real version in users' hands in weeks, on foundations that hold up when it works.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>The team has outgrown its spreadsheets</h3>
          <span class="stack">Excavation · Manufacturing · Marketing</span>
        </div>
        <div class="row-body">
          <p>Five tools, a dozen Excel files, and no agreement on which one is current. I spend time with the people doing the work, then build the single system that replaces the pile.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>The build has stalled, or nobody senior is steering</h3>
          <span class="stack">Healthcare · Marketing · Web3</span>
        </div>
        <div class="row-body">
          <p>A feature that won't land, a codebase that creaks, or a team with no senior voice in the room. I carry the technical decisions and keep everyone else unblocked. I've hired and mentored the people who inherit the code.</p>
        </div>
      </li>
    </ul>
  </div>
</section>

<section id="contact">
  <div class="wrap">
    <div class="section-head">
      <p class="label">Contact</p>
      <h2>What's slowing you down?</h2>
      <p>Tell me about the thing that keeps costing you time or sleep. Don't worry about having it all figured out. I'll reply within a day with honest thoughts on scope, timeline, and whether I'm the right fit.</p>
    </div>
    <dl class="details">
      <dt>Email</dt>
      <dd><a href="mailto:{{ site.email }}">{{ site.email }}</a></dd>
      <dt>LinkedIn</dt>
      <dd><a href="https://www.linkedin.com/in/andr-drgm/" target="_blank" rel="noopener">andr-drgm</a></dd>
      <dt>GitHub</dt>
      <dd><a href="https://github.com/andr-drgm" target="_blank" rel="noopener">andr-drgm</a></dd>
      <dt>Location</dt>
      <dd>Sibiu, Romania (remote, CET)</dd>
    </dl>
  </div>
</section>
