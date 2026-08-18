---
layout: default
title: Home
description: Andrei Dragomir — I build internal platforms, automation systems and MVPs that reach real users.
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
        <h1>Most projects don't fail on the code.</h1>
        <p class="lede" style="margin-top:1.25rem">They fail on scope, on the wrong problem, on the thing nobody wrote down. I build internal platforms, automation systems and MVPs that reach real users — for teams that don't need more features, they need someone to work out what's actually in the way first.</p>
      </div>
      <img class="portrait" src="/assets/img/andrei.jpg" alt="Andrei Dragomir" width="720" height="900" decoding="async">
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Approach</p>
      <h2>Three habits, not a methodology.</h2>
    </div>
    <ol class="numbered">
      <li>
        <h3>Start with the problem</h3>
        <p>Projects fail because nobody pinned down what the business is actually trying to move. I start there, then work backwards to the smallest thing that gets it done.</p>
      </li>
      <li>
        <h3>Delete more than I add</h3>
        <p>Most of my best work is deletion — a "custom platform" that turns out to be three forms and a cron job, a tangle of spreadsheets replaced by one screen someone actually opens.</p>
      </li>
      <li>
        <h3>Build for whoever inherits it</h3>
        <p>I've hired and mentored the people who take over the code, which is mostly a lesson in writing things a future teammate won't curse me for.</p>
      </li>
    </ol>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Services</p>
      <h2>How I can help</h2>
    </div>
    <ul class="rows">
      <li>
        <div>
          <h3>Idea → launched MVP</h3>
          <span class="stack">Solo founders · Early-stage startups</span>
        </div>
        <div class="row-body">
          <p>Clients come with a validated idea but nothing real users can touch, and every month of hesitation costs them. I pin down the one thing that has to be proven, cut everything else, and ship a real version in weeks — on foundations solid enough to grow on.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Operations stuck on spreadsheets</h3>
          <span class="stack">Excavation · Manufacturing · Marketing</span>
        </div>
        <div class="row-body">
          <p>A team juggling five tools and Excel files, losing data, making errors, with no single source of truth. I centralize the flow into a platform shaped around how they already work and automate the repetitive step, rather than forcing a new process on them.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Code that needs rescuing</h3>
          <span class="stack">Healthcare · Marketing · Web3</span>
        </div>
        <div class="row-body">
          <p>A codebase that's creaking, a feature that's stalled, or a gap where a senior pair of hands should be until launch. I plug into the existing stack, stabilize what's fragile, and deliver — without rewriting everything for the sake of it.</p>
        </div>
      </li>
    </ul>
    <p class="section-foot"><a href="/projects/">See what I've built →</a></p>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Contact</p>
      <h2>What's slowing you down?</h2>
      <p>Tell me about the thing that keeps costing you time or sleep — don't worry about having it all figured out. I'll reply within a day with honest thoughts on scope, timeline, and whether I'm the right fit.</p>
    </div>
    <dl class="details">
      <dt>Email</dt>
      <dd><a href="mailto:{{ site.email }}">{{ site.email }}</a></dd>
      <dt>LinkedIn</dt>
      <dd><a href="https://www.linkedin.com/in/andr-drgm/" target="_blank" rel="noopener">andr-drgm</a></dd>
      <dt>GitHub</dt>
      <dd><a href="https://github.com/andr-drgm" target="_blank" rel="noopener">andr-drgm</a></dd>
      <dt>Location</dt>
      <dd>Sibiu, Romania — remote, CET</dd>
      <dt>Education</dt>
      <dd>BSc Computer Science, Babeș-Bolyai University, Cluj-Napoca</dd>
      <dt>Reply time</dt>
      <dd>Within a day</dd>
    </dl>
  </div>
</section>
