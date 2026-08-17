---
layout: default
title: Work
permalink: /work/
description: Projects, case studies, and experience — Andrei Dragomir, software engineer.
---

{% assign case_study = "/writing/selected-work/" %}

<section class="hero">
  <div class="wrap">
    <p class="eyebrow">Work</p>
    <h1>Nine years of shipping, mostly for teams<br>who needed one screen instead of five tools.</h1>
    <p class="lede" style="margin-top:1.25rem;max-width:38rem">Nearly every project reaches me with the same underlying issue — nobody nailed down what the business is actually trying to move. That's where I start, and it's the thread running through all of this.</p>
    <div class="cta">
      <a class="btn btn-primary" href="{{ case_study }}">Read the case studies</a>
      <a class="btn btn-ghost" href="mailto:andrei.dragomir.contact@gmail.com">Get in touch</a>
    </div>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Projects</p>
      <h2>What I've built</h2>
      <p>Live links and repos where they exist. Each card goes to the full case study — problem, approach, outcome.</p>
    </div>
    <div class="cards">
      {%- for project in site.data.projects %}
        {% include project-card.html project=project post_url=case_study %}
      {%- endfor %}
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Services</p>
      <h2>How I can help</h2>
    </div>
    <div class="skill-grid">
      <div class="skill-card reveal">
        <h3>Idea → launched MVP</h3>
        <p><strong>What clients come with:</strong> a validated idea but nothing real users can touch, and every month of hesitation costs them.</p>
        <p><strong>How I approach it:</strong> pin down the one thing that has to be proven, cut everything else, ship a real version in weeks — on foundations solid enough to grow on.</p>
        <div class="chips"><span class="chip">Solo founders</span><span class="chip">Early-stage startups</span></div>
      </div>
      <div class="skill-card reveal">
        <h3>Operations stuck on spreadsheets</h3>
        <p><strong>What clients come with:</strong> a team juggling five tools and Excel files, losing data, making errors, with no single source of truth.</p>
        <p><strong>How I approach it:</strong> centralize the flow into a platform shaped around how they already work, and automate the repetitive step — rather than forcing a new process on them.</p>
        <div class="chips"><span class="chip">Excavation</span><span class="chip">Manufacturing</span><span class="chip">Marketing</span></div>
      </div>
      <div class="skill-card reveal">
        <h3>Code that needs rescuing</h3>
        <p><strong>What clients come with:</strong> a codebase that's creaking, a feature that's stalled, or a gap where a senior pair of hands should be until launch.</p>
        <p><strong>How I approach it:</strong> plug into the existing stack, stabilize what's fragile, and deliver — without rewriting everything for the sake of it.</p>
        <div class="chips"><span class="chip">Healthcare</span><span class="chip">Marketing</span><span class="chip">Web3</span></div>
      </div>
    </div>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Experience</p>
      <h2>Where I've worked</h2>
    </div>
    <div class="timeline">
      <div class="job reveal">
        <h3>Full-Stack Engineer — Pastrac</h3>
        <span class="meta">Duty Ventures · Apr 2026 — present</span>
        <p>Built a React Native iOS app for tagging, tracking and sharing locations on a personalized map, with Supabase powering real-time sync, auth and storage. Shipped to the App Store.</p>
        <div class="chips"><span class="chip">React Native</span><span class="chip">Supabase</span><span class="chip">iOS</span></div>
      </div>
      <div class="job reveal">
        <h3>Software Engineer — Archeo</h3>
        <span class="meta">Duty Ventures · Feb 2025 — May 2026</span>
        <p>Built an internal platform from scratch in Rails — database architecture and a responsive UI for both office and field use — centralizing operational data across excavation sites and employee management. It replaced dozens of Excel sheets where nobody was certain which file was current.</p>
        <div class="chips"><span class="chip">Ruby on Rails</span><span class="chip">TailwindCSS</span><span class="chip">PostgreSQL</span></div>
      </div>
      <div class="job reveal">
        <h3>Software Developer — Internal R&amp;T Product Platform</h3>
        <span class="meta">Duty Ventures · Aug 2024 — May 2026</span>
        <p>Worked within a large team on a complex internal platform for a multinational personal-care manufacturer, tracking products through research and testing before they reached market.</p>
        <div class="chips"><span class="chip">Django</span><span class="chip">React</span><span class="chip">Python</span></div>
      </div>
      <div class="job reveal">
        <h3>Lead Software Engineer — DPA Services</h3>
        <span class="meta">Duty Ventures · Nov 2022 — Aug 2024</span>
        <p>Led the development team — recruiting and mentoring new programmers — while building Puppeteer-based internal tools that automated repetitive work for the agency's virtual assistants, and running the servers and databases behind them.</p>
        <div class="chips"><span class="chip">TypeScript</span><span class="chip">Puppeteer</span><span class="chip">Firebase</span><span class="chip">Stripe</span></div>
      </div>
      <div class="job reveal">
        <h3>Software Engineer — Med Prep</h3>
        <span class="meta">Duty Ventures · Jul 2022 — Nov 2022</span>
        <p>Built a scalable online testing platform giving medical students access to large question banks and timed exams, optimizing performance for high concurrent load around exam season.</p>
        <div class="chips"><span class="chip">Ruby on Rails</span><span class="chip">Stripe</span></div>
      </div>
      <div class="job reveal">
        <h3>Software Developer — Telemed</h3>
        <span class="meta">Duty Ventures · Apr 2022 — Jul 2022</span>
        <p>Built mobile apps and backend for an appointment-booking platform used by US clinics, integrating Docusign so intake paperwork was signed without a separate email thread.</p>
        <div class="chips"><span class="chip">React Native</span><span class="chip">Ruby on Rails</span><span class="chip">Docusign</span></div>
      </div>
      <div class="job reveal">
        <h3>SAP ABAP Developer — Intern</h3>
        <span class="meta">NTT DATA Romania · Sep 2021 — Dec 2021</span>
        <p>Enterprise software experience building gas-station management software in SAP ABAP — transaction management, data validation, and integration with external systems for real-time processing.</p>
        <div class="chips"><span class="chip">SAP ABAP</span></div>
      </div>
      <div class="job reveal">
        <h3>Android Developer — Intern</h3>
        <span class="meta">TerraConnect · Jun 2021 — Aug 2021</span>
        <p>Built authentication, event creation and real-time notifications for a Kotlin Android app connecting sports enthusiasts and helping them organize events.</p>
        <div class="chips"><span class="chip">Kotlin</span><span class="chip">Android</span></div>
      </div>
      <div class="job reveal">
        <h3>Web Developer — Freelance</h3>
        <span class="meta">Self-employed · Jun 2020 — Aug 2020</span>
        <p>Worked with small local businesses to build their first real web presence — including DSS Inox, still live today.</p>
        <div class="chips"><span class="chip">Full-Stack</span><span class="chip">Web</span></div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head reveal">
      <p class="eyebrow">Stack</p>
      <h2>What I reach for</h2>
    </div>
    <div class="skill-grid">
      <div class="skill-card reveal">
        <h3>Backend &amp; data</h3>
        <div class="chips">
          <span class="chip">Ruby on Rails</span><span class="chip">Django</span><span class="chip">Node.js</span>
          <span class="chip">Python</span><span class="chip">Ruby</span><span class="chip">PostgreSQL</span>
          <span class="chip">Firebase</span><span class="chip">Supabase</span>
        </div>
      </div>
      <div class="skill-card reveal">
        <h3>Frontend &amp; mobile</h3>
        <div class="chips">
          <span class="chip">TypeScript</span><span class="chip">React</span><span class="chip">Next.js</span>
          <span class="chip">React Native</span><span class="chip">TailwindCSS</span><span class="chip">Kotlin</span>
        </div>
      </div>
      <div class="skill-card reveal">
        <h3>Infrastructure &amp; Web3</h3>
        <div class="chips">
          <span class="chip">Docker</span><span class="chip">CI/CD</span><span class="chip">Git</span>
          <span class="chip">Puppeteer</span><span class="chip">Stripe</span><span class="chip">Solana</span>
          <span class="chip">Solidity</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="band">
  <div class="wrap">
    <div class="contact-box reveal">
      <div>
        <p class="eyebrow">Contact</p>
        <h2>Let's build something</h2>
        <p class="lede">Remote, working with clients worldwide. BSc Computer Science, Babeș-Bolyai University, Cluj-Napoca.</p>
        <div class="cta">
          <a class="btn btn-primary" href="mailto:andrei.dragomir.contact@gmail.com">andrei.dragomir.contact@gmail.com</a>
          <a class="btn btn-ghost" href="https://github.com/andr-drgm" target="_blank" rel="noopener">GitHub</a>
        </div>
      </div>
      <img class="portrait" src="/assets/img/andrei.jpg" alt="Andrei Dragomir" width="720" height="900" loading="lazy" decoding="async">
    </div>
  </div>
</section>
