---
layout: default
title: Home
---

{% assign case_study = "/writing/selected-work/" %}

<section class="hero">
  <div class="wrap">
    <p class="eyebrow">Internal platforms · automation · MVPs</p>
    <h1>Most projects don't fail on the code.</h1>
    <p class="lede">They fail on scope, on the wrong problem, on the thing nobody wrote down. I build internal platforms, automation systems, and MVPs that reach real users — for teams that don't need more features, they need someone to work out what's actually in the way first.</p>
    <div class="cta">
      <a class="btn btn-primary" href="mailto:andrei.dragomir.contact@gmail.com">Tell me what's slowing you down</a>
      <a class="btn btn-ghost" href="/work/">See the work</a>
    </div>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Selected work</p>
      <h2>Three problems, and what changed after</h2>
      <p>An excavation company that couldn't say which spreadsheet was current, an iOS app shipped to the App Store, and the testing platform behind a Swiss medical-school prep school.</p>
    </div>
    <div class="cards">
      {%- for project in site.data.projects %}
        {%- if project.featured %}
          {% include project-card.html project=project post_url=case_study %}
        {%- endif %}
      {%- endfor %}
    </div>
    <p class="section-foot reveal"><a href="/work/">All projects and experience →</a></p>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Approach</p>
      <h2>Three habits, not a methodology.</h2>
    </div>
    <div class="skill-grid">
      <div class="skill-card reveal">
        <h3>Start with the problem</h3>
        <p>Projects fail because nobody pinned down what the business is actually trying to move. I start there, then work backwards to the smallest thing that gets it done.</p>
      </div>
      <div class="skill-card reveal">
        <h3>Delete more than I add</h3>
        <p>Most of my best work is deletion — a "custom platform" that turns out to be three forms and a cron job, a tangle of spreadsheets replaced by one screen someone actually opens.</p>
      </div>
      <div class="skill-card reveal">
        <h3>Build for whoever inherits it</h3>
        <p>I've hired and mentored the people who take over the code, which is mostly a lesson in writing things a future teammate won't curse me for.</p>
      </div>
    </div>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Writing</p>
      <h2>Notes from the work</h2>
    </div>
    <ul class="posts reveal">
      {%- for post in site.posts limit: 5 %}
      <li>
        <a href="{{ post.url }}">
          <span class="meta">{{ post.date | date: "%b %Y" }}</span>
          <strong>{{ post.title }}</strong>
          {% if post.description %}<em>{{ post.description }}</em>{% endif %}
        </a>
      </li>
      {%- endfor %}
    </ul>
    {% if site.posts.size > 5 %}<p class="section-foot"><a href="/writing/">All posts →</a></p>{% endif %}
  </div>
</section>

<section>
  <div class="wrap">
    <div class="contact-box reveal">
      <div>
        <p class="eyebrow">Contact</p>
        <h2>What's slowing you down?</h2>
        <p class="lede">Tell me about the thing that keeps costing you time or sleep — don't worry about having it all figured out. I'll reply within a day with honest thoughts on scope, timeline, and whether I'm the right fit.</p>
        <div class="cta">
          <a class="btn btn-primary" href="mailto:andrei.dragomir.contact@gmail.com">andrei.dragomir.contact@gmail.com</a>
          <a class="btn btn-ghost" href="https://www.linkedin.com/in/andr-drgm/" target="_blank" rel="noopener">LinkedIn</a>
        </div>
      </div>
      <img class="portrait" src="/assets/img/andrei.jpg" alt="Andrei Dragomir" width="720" height="900" loading="lazy" decoding="async">
    </div>
  </div>
</section>
