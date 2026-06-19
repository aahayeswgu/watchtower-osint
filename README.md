# WatchTower

I started WatchTower after watching a run of "teen takeover" events blow up across Florida
beaches and malls in 2026, including one close to home. These gatherings get advertised in the
open before they happen, and then the original posts tend to vanish. I wanted to find out whether
a small, public-only tool could catch that advertising early and turn it into something a person
could actually act on. This one is a passion project. I built it because I wanted to.

WatchTower reads public, open-source signals, separates the real disorder-trend events from the
benign look-alikes (a city parks-and-rec teen night is not the same thing), reads the flyers, and
writes it all up as a short, structured intelligence brief. Public data only. Events, never
individuals. No facial recognition.

## A look at the output

<img src="docs/cover.png" width="430">

<img src="docs/assessment.png" width="430">

<img src="docs/forward.png" width="430">

## How it's put together

High level only. The actual collection logic, prompts, and scoring are private.

```
watchtower/
├── collect/     pull public, open-source signals across platforms
├── classify/    sort real trend events from benign look-alikes, with a confidence level
├── extract/     read flyer images for place / date / time
├── score/       rank events by how many independent public sources agree
└── report/      render the OSINT brief (PDF)
```

## Ground rules I built in

- Public, logged-out sources only. No logins, no fake accounts.
- No facial recognition or biometrics, ever.
- Events, not individuals.
- Links back to public sources, minimal retention.
- Not crime prediction, and not meant for evidence.

## Tech

Python, a large-language model for reading flyer images and sorting signals, public search, and
automated PDF generation.

## Status

Working prototype, built and tested on real Florida events. The implementation and methodology
are private; this repo is an overview of what it does and why I made it.

Built by Tracecast LLC.
