---
layout: default
title: Home
---

{% assign case_study = "/writing/selected-work/" %}

<section class="hero">
  <div class="wrap">
    <p class="eyebrow">Internal platforms · automation · MVPs</p>
    <h1>Most projects don't fail on the code.</h1>
    <div class="hero-body">
      <div>
        <p class="lede">They fail on scope, on the wrong problem, on the thing nobody wrote down. I build internal platforms, automation systems, and MVPs that reach real users — for teams that don't need more features, they need someone to work out what's actually in the way first.</p>
        <div class="cta">
          <a class="btn btn-primary" href="mailto:{{ site.email }}">Tell me what's slowing you down</a>
          <a class="btn btn-ghost" href="/work/">See the work</a>
        </div>
      </div>
      <img class="portrait" src="/assets/img/andrei.jpg" alt="Andrei Dragomir" width="720" height="900" decoding="async">
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
    {%- comment -%}
    Archeo spans the row with its schematic large — the diagram is the argument, and
    at card width you can't read either state. Pastrac and Med Prep are shipped, public
    products, so they show the real thing and sit as a pair beneath.
    {%- endcomment -%}
    <div class="cards cards-pair">
      {%- for project in site.data.projects %}
        {%- if project.featured %}
          {% include project-card.html project=project post_url=case_study %}
        {%- endif %}
      {%- endfor %}
    </div>
    <p class="section-foot reveal"><a href="/work/">All projects and experience →</a></p>
  </div>
</section>

{%- comment -%}
The one full-bleed green section on the page, so the accent appears at scale
somewhere and not only inside buttons. Three annotated lines, not three boxes.
{%- endcomment -%}
<section class="band-accent">
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Approach</p>
      <h2>Three habits, not a methodology.</h2>
    </div>
    <ol class="habits">
      <li class="reveal">
        <span class="habits-n">01</span>
        <h3>Start with the problem</h3>
        <p>Projects fail because nobody pinned down what the business is actually trying to move. I start there, then work backwards to the smallest thing that gets it done.</p>
      </li>
      <li class="reveal">
        <span class="habits-n">02</span>
        <h3>Delete more than I add</h3>
        <p>Most of my best work is deletion — a "custom platform" that turns out to be three forms and a cron job, a tangle of spreadsheets replaced by one screen someone actually opens.</p>
      </li>
      <li class="reveal">
        <span class="habits-n">03</span>
        <h3>Build for whoever inherits it</h3>
        <p>I've hired and mentored the people who take over the code, which is mostly a lesson in writing things a future teammate won't curse me for.</p>
      </li>
    </ol>
  </div>
</section>

{%- comment -%}
A "Notes from the work" heading over a single item that isn't a note reads thinner
than no section. It comes back on its own once a second post exists.
{%- endcomment -%}
{% if site.posts.size > 1 %}
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
{% endif %}

<section>
  <div class="wrap">
    <div class="contact-box reveal">
      <div>
        <p class="eyebrow">Contact</p>
        <h2>What's slowing you down?</h2>
        <p class="lede">Tell me about the thing that keeps costing you time or sleep — don't worry about having it all figured out. I'll reply within a day with honest thoughts on scope, timeline, and whether I'm the right fit.</p>
        <div class="cta">
          <a class="btn btn-primary" href="mailto:{{ site.email }}">Start the conversation</a>
        </div>
      </div>
      <dl class="contact-details">
        <dt>Email</dt>
        <dd><a href="mailto:{{ site.email }}">{{ site.email }}</a></dd>
        <dt>LinkedIn</dt>
        <dd><a href="https://www.linkedin.com/in/andr-drgm/" target="_blank" rel="noopener">andr-drgm</a></dd>
        <dt>GitHub</dt>
        <dd><a href="https://github.com/andr-drgm" target="_blank" rel="noopener">andr-drgm</a></dd>
        <dt>Location</dt>
        <dd>Sibiu, Romania — remote, CET</dd>
        <dt>Reply time</dt>
        <dd>Within a day</dd>
      </dl>
    </div>
  </div>
</section>
