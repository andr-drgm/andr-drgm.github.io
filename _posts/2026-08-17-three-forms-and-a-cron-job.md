---
layout: post
title: "Three forms and a cron job"
description: Most custom platforms are smaller than the document describing them.
---

Every few months someone sends me a spec for a custom platform. Twelve pages, a
roles matrix, a section headed *Phase 2*. And nearly every time, the thing the
business actually needs to do fits in three forms and a cron job.

![A sprawling spec collapsing into three forms and a cron job](/assets/posts/three-forms-and-a-cron.svg)

That isn't a dig at the person who wrote the spec. A long document is what
happens when nobody has been allowed to ask which part earns its keep. The
spreadsheet everyone complains about is doing four jobs; the spec dutifully
describes all four, plus the six more someone might want later.

## Find the thing that has to be true

So the first question I ask isn't *what should it do* — it's what has to be true
for this to be worth building at all. Usually there's exactly one:

- Field staff can log a job without calling the office.
- Finance sees yesterday's numbers before the morning meeting.
- A customer can book without an email thread.

Build that. Ship it. The rest of the spec either gets requested by a real user
in week three, or it quietly turns out nobody wanted it — and you saved a month.

## The cron job is not a compromise

The part people push back on is the boring machinery. Surely a real platform
gets a queue, a worker pool, a dashboard for the worker pool?

```
0 3 * * *  cd /srv/app && ./bin/sync >> log/sync.log 2>&1
```

That line has run nightly for three years at one client. It has never paged
anyone. When it eventually needs to run every ten minutes instead of nightly,
changing it is a one-character edit — and *that's* the moment to reach for a
queue, not before.

Dull software that runs for three years beats clever software you have to
babysit. Most of my best work is what I talked someone out of building.
