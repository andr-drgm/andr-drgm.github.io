---
layout: post
title: "Selected work, 2020–2026"
description: Nine projects, what each one was actually for, and what changed after it shipped.
# No og:image override — the schematics are SVG, which social cards won't render.
---

Portfolios usually show you the screen and skip the part that matters — what the thing was
*for*, and what was true afterwards that wasn't true before. So this is the long version:
problem, approach, outcome, for the work I'd want to be judged on.

Three of these are what I'm actively building right now — [Pastrac](#pastrac),
[Collaborators](#collaborators), and [Med Prep](#medprep). The rest run backwards from there.
If you want the scannable version instead, [/work/](/work/) has the cards.

## Pastrac {#pastrac}

<div class="facts" markdown="0">
  <span>React Native · Supabase · iOS</span>
  <a href="https://www.pastrac.com/" target="_blank" rel="noopener">pastrac.com ↗</a>
  <a href="https://apps.apple.com/us/app/pastrac-app/id6754891045" target="_blank" rel="noopener">App Store ↗</a>
</div>

![The Pastrac site, showing the iOS app over a live map](/assets/work/pastrac.jpg){: width="1200" height="736"}

**Problem.** Check-ins are a solved problem and a boring one — a pin with a timestamp tells you
nothing in two years. What people actually want is the memory attached to the place, and control
over who gets to see it.

**Approach.** A React Native app built around the map rather than a feed. You tap anywhere on the
live map or search a place, write what happened, attach photos from library or camera, and tag it
— life event, food, music. Then you choose the audience: public, family, or just friends. Supabase
handles auth, storage and real-time sync, which meant no backend to babysit for a product still
finding its shape.

The design constraint that mattered: the whole flow, from opening the app to publishing, is three
steps. Anything that added a fourth got cut.

**Outcome.** Shipped and live on the App Store.

## Collaborators {#collaborators}

<div class="facts" markdown="0">
  <span>Next.js 14 · Solana · Prisma · NextAuth</span>
  <a href="https://collaborators.build" target="_blank" rel="noopener">collaborators.build ↗</a>
  <a href="https://github.com/andr-drgm/collaborators" target="_blank" rel="noopener">Code ↗</a>
</div>

![The Collaborators landing page](/assets/work/collaborators.jpg){: width="1200" height="687"}

**Problem.** Open-source maintainers have no good way to pay the person who fixed the issue.
Contributors have no durable, verifiable record of the work they did. Both sides fall back on
goodwill, which doesn't pay rent.

**Approach.** Tie rewards to activity that can actually be verified. Contributors log in with
GitHub and link a Solana wallet; the platform tracks real contributions rather than
self-reported ones. Maintainers connect a repo and set a bounty directly on an open issue, and
once the work is solved and reviewed the funds go straight to the contributor's wallet. Verified
contributions also mint NFT badges, so the record outlives any one platform.

**Outcome.** The bounty system is live, and the project went through the Cypherpunk Hackathon
powered by Colosseum. It's the clearest example of me taking something from zero to a working
product in a domain — on-chain payments — where "mostly working" isn't good enough.

## Med Prep {#medprep}

<div class="facts" markdown="0">
  <span>Ruby on Rails · Stripe · PostgreSQL</span>
  <a href="https://www.medprep.ch/" target="_blank" rel="noopener">medprep.ch ↗</a>
</div>

![The Med Prep website](/assets/work/medprep.jpg){: width="1200" height="736"}

**Problem.** Med Prep is a Swiss prep school in Geneva and Lausanne that gets medical students
through a brutal first year. Their teaching was excellent and their delivery was manual — the
question banks, mock exams and scoring all needed to become software that thousands of students
could hit at once, hardest right before exams.

**Approach.** A Rails testing platform built for the load pattern rather than the average: large
question banks organised by subject, timed exams under real conditions, detailed scoring, and
subscriptions through Stripe. Performance work focused on the concurrency spike around exam
season, because that's the only moment when being slow actually costs the school anything.

**Outcome.** The platform carries the paid side of a school that has worked with over 13,000
students since 2009 — their figures, not mine. Practice, mock exams and scoring stopped being
something staff assembled by hand.

## Archeo {#archeo}

<div class="facts" markdown="0">
  <span>Ruby on Rails · TailwindCSS · PostgreSQL</span>
  <span>Internal — no public link</span>
</div>

![Loose spreadsheets and PDF reports consolidated into one records system](/assets/work/archeo.svg){: width="1200" height="675"}

**Problem.** An excavation company in Saudi Arabia was running its operations on dozens of Excel
sheets and a pile of third-party tools. It worked, until nobody could say with confidence which
file was the latest version. That's not a spreadsheet problem, it's a truth problem.

**Approach.** I built the platform from scratch in Rails — database architecture first, because
the whole point was one authoritative record — with a TailwindCSS UI that had to work on an
office monitor and on a phone at a dig site. Sites, crews, hours and employee management in one
place, shaped around how the team already worked instead of a process imposed on them.

**Outcome.** It replaced the Excel-and-PDF-report workflow the company had been running on. The
data lives in one system now, so "which version is current" stopped being a question anyone asks.

## R&T product platform {#rt-platform}

<div class="facts" markdown="0">
  <span>Django · React · Python</span>
  <span>Internal — no public link</span>
</div>

![Products moving through research and testing stages toward market](/assets/work/rt-platform.svg){: width="1200" height="675"}

**Problem.** A multinational personal-care manufacturer needed to see where every product was in
the pipeline between research and market — formulation, stability testing, panel testing,
approval — across a lot of concurrent products and a lot of teams.

**Approach.** Part of a large engineering team on a Django and React platform tracking products
through each research and testing stage. Working in a big team on a system this size is mostly a
discipline exercise: your slice has to be legible to people who will touch it long after you've
moved on.

**Outcome.** Where a product sits between formulation and market became something you look up
rather than ask around for. No headline number here — I don't have one I can stand behind, and
this is the wrong page to invent one.

## Agency automation {#dpa}

<div class="facts" markdown="0">
  <span>TypeScript · Puppeteer · Firebase · Stripe</span>
  <span>Internal — no public link</span>
</div>

![Repetitive browser work moved from people onto scheduled automation](/assets/work/dpa-automation.svg){: width="1200" height="675"}

**Problem.** A digital marketing agency had virtual assistants doing hundreds of identical
browser actions a day — copy, paste, repeat. Expensive, error-prone, and demoralising for the
people doing it.

**Approach.** Custom Puppeteer tooling that did the repetitive browser work directly, including
reverse-engineering the existing apps involved to drive them reliably. I also ran the servers and
databases behind it, and led the development team — recruiting and mentoring the programmers who
would maintain the tooling after me.

**Outcome.** The manual, repetitive browser work moved off the virtual assistants and onto
tooling that ran it on a schedule. The team kept the interesting half of the job.

## DSS Inox {#dss-inox}

<div class="facts" markdown="0">
  <span>JavaScript · Firebase Hosting</span>
  <a href="https://dss-inox-website.web.app/" target="_blank" rel="noopener">Live site ↗</a>
  <a href="https://github.com/andr-drgm/dss-inox-website" target="_blank" rel="noopener">Code ↗</a>
</div>

![Brushed stainless steel panels](/assets/work/dss-inox.svg){: width="1200" height="675"}

**Problem.** A stainless-steel fabrication business in Mediaș had no web presence at all. Their
customers were finding them by word of mouth and phone calls.

**Approach.** A straightforward service site — what they make, why stainless holds up, and how to
reach them — on Firebase Hosting so there was nothing to maintain and nothing to pay for.

**Outcome.** Live since 2020 and still up, which for a small-business site is the whole
specification. This is the earliest work here and it shows, but it's honest: not every problem
needs a platform.

## Crypto Staking Calculator {#staking-calculator}

<div class="facts" markdown="0">
  <span>React 18 · Material UI</span>
  <a href="https://andrei-dragomir.com/crypto-staking-calculator/">Live demo ↗</a>
  <a href="https://github.com/andr-drgm/crypto-staking-calculator" target="_blank" rel="noopener">Code ↗</a>
</div>

![A retro arcade styled staking reward calculator](/assets/work/staking-calculator.jpg){: width="1200" height="687"}

**Problem.** Staking calculators all quote you an APR and let you assume that's what you'll
earn. The interesting number is what compounding does to it, and almost nothing shows the two
side by side.

**Approach.** Daily-through-yearly reward estimates with a plain-APR versus compounding
comparison, wrapped in a deliberately retro arcade interface. The personality is the point: a
self-contained side project is where you get to prove you can finish something and make it feel
like an actual product rather than a form.

**Outcome.** Shipped, live, and self-contained end to end.

## WallApp {#wallapp}

<div class="facts" markdown="0">
  <span>Android · Java</span>
  <a href="https://github.com/andr-drgm/WallApp-Wallpaper" target="_blank" rel="noopener">Code ↗</a>
</div>

![A phone showing a grid of wallpapers by local artists](/assets/work/wallapp.svg){: width="1200" height="675"}

**Problem.** Romanian digital artists were posting work into social feeds that buried it in a
day. A wallpaper is a better home for that work than a timeline — it's what someone looks at
fifty times a day.

**Approach.** A native Android app where the artist is a first-class object: set a wallpaper,
follow a creator, save favourites. Built so browsing by artist felt as natural as browsing by
image.

**Outcome.** Published to Google Play and used. The listing is no longer live — worth stating
plainly rather than leaving a dead link on a portfolio — but the source is still up.

## Early work {#early}

![An exchange rate web app with live currency conversion](/assets/work/exchange-rate.jpg){: width="1200" height="687"}

The [exchange-rate app](https://andrei-dragomir.com/exchange-rate/) is from high school: live
currency conversion, a converter, and a rate chart. It's still deployed, and I keep it that way
on purpose. It's the first thing I built that a stranger could use without me standing next to
them, which is a line worth remembering.

Before the work above there were also two shorter engagements worth naming: **Telemed**, an
appointment-booking platform for US clinics where I built the mobile apps and backend and wired
up Docusign so intake paperwork stopped being an email thread; and an **SAP ABAP** internship at
NTT DATA building gas-station management software, which is where I learned what enterprise
software costs to change.

---

If any of this looks like the problem you're currently sitting on,
[tell me what's slowing you down](mailto:andrei.dragomir.contact@gmail.com). I reply within a day.
