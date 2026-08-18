---
layout: default
title: Projects
permalink: /projects/
description: Projects, case studies and experience — Andrei Dragomir, software engineer.
---

{% assign case_study = "/blog/selected-work/" %}

<section>
  <div class="wrap">
    <div class="page-head">
      <h1>Nine years of shipping, mostly for teams who needed one screen instead of five tools.</h1>
      <p class="lede">Nearly every project reaches me with the same underlying issue — nobody nailed down what the business is actually trying to move. That's where I start, and it's the thread running through all of this.</p>
      <p class="section-foot"><a href="{{ case_study }}">Read the long version →</a></p>
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Projects</p>
      <h2>What I've built</h2>
      <p>Live links and repos where they exist. Each name goes to the full case study — problem, approach, outcome.</p>
    </div>
    <ul class="rows rows--media">
      {%- for project in site.data.projects %}
        {% include project-row.html project=project post_url=case_study %}
      {%- endfor %}
    </ul>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <p class="label">Experience</p>
      <h2>Where I've worked</h2>
    </div>
    <ul class="rows">
      <li>
        <div>
          <h3>Full-Stack Engineer — Pastrac</h3>
          <span class="meta">Duty Ventures · Apr 2026 — present</span>
          <span class="stack">React Native · Supabase · iOS</span>
        </div>
        <div class="row-body">
          <p>Built a React Native iOS app for tagging, tracking and sharing locations on a personalized map, with Supabase powering real-time sync, auth and storage. Shipped to the App Store.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Software Engineer — Archeo</h3>
          <span class="meta">Duty Ventures · Feb 2025 — May 2026</span>
          <span class="stack">Ruby on Rails · TailwindCSS · PostgreSQL</span>
        </div>
        <div class="row-body">
          <p>Built an internal platform from scratch in Rails — database architecture and a responsive UI for both office and field use — centralizing operational data across excavation sites and employee management. It replaced dozens of Excel sheets where nobody was certain which file was current.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Software Developer — Internal R&amp;T Product Platform</h3>
          <span class="meta">Duty Ventures · Aug 2024 — May 2026</span>
          <span class="stack">Django · React · Python</span>
        </div>
        <div class="row-body">
          <p>Worked within a large team on a complex internal platform for a multinational personal-care manufacturer, tracking products through research and testing before they reached market.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Lead Software Engineer — DPA Services</h3>
          <span class="meta">Duty Ventures · Nov 2022 — Aug 2024</span>
          <span class="stack">TypeScript · Puppeteer · Firebase · Stripe</span>
        </div>
        <div class="row-body">
          <p>Led the development team — recruiting and mentoring new programmers — while building Puppeteer-based internal tools that automated repetitive work for the agency's virtual assistants, and running the servers and databases behind them.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Software Engineer — Med Prep</h3>
          <span class="meta">Duty Ventures · Jul 2022 — Nov 2022</span>
          <span class="stack">Ruby on Rails · Stripe</span>
        </div>
        <div class="row-body">
          <p>Built a scalable online testing platform giving medical students access to large question banks and timed exams, optimizing performance for high concurrent load around exam season.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Software Developer — Telemed</h3>
          <span class="meta">Duty Ventures · Apr 2022 — Jul 2022</span>
          <span class="stack">React Native · Ruby on Rails · Docusign</span>
        </div>
        <div class="row-body">
          <p>Built mobile apps and backend for an appointment-booking platform used by US clinics, integrating Docusign so intake paperwork was signed without a separate email thread.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>SAP ABAP Developer — Intern</h3>
          <span class="meta">NTT DATA Romania · Sep 2021 — Dec 2021</span>
          <span class="stack">SAP ABAP</span>
        </div>
        <div class="row-body">
          <p>Enterprise software experience building gas-station management software in SAP ABAP — transaction management, data validation, and integration with external systems for real-time processing.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Android Developer — Intern</h3>
          <span class="meta">TerraConnect · Jun 2021 — Aug 2021</span>
          <span class="stack">Kotlin · Android</span>
        </div>
        <div class="row-body">
          <p>Built authentication, event creation and real-time notifications for a Kotlin Android app connecting sports enthusiasts and helping them organize events.</p>
        </div>
      </li>
      <li>
        <div>
          <h3>Web Developer — Freelance</h3>
          <span class="meta">Self-employed · Jun 2020 — Aug 2020</span>
          <span class="stack">Full-Stack · Web</span>
        </div>
        <div class="row-body">
          <p>Worked with small local businesses to build their first real web presence — including DSS Inox, still live today.</p>
        </div>
      </li>
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
