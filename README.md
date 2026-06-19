# WatchTower

WatchTower looks through public, open-source signals to find gatherings that are being
advertised in the open (for example, the Florida "teen takeover" events), and turns what it
finds into a structured report: which events were advertised, where, how many separate public
sources mention each one, and how confident the read is.

It only uses public posts. It flags events, not people. No facial recognition, no biometrics.

<img src="docs/cover.png" alt="WatchTower report cover" width="500">

## What's in the report

- A short summary of what was found, with the headline numbers
- Charts: activity by month, by city, by outcome, by venue type
- An event log with source counts and a confidence rating on each event
- Flyer reading that pulls the place, date, and time straight off public flyer images
- A live scan of what is being advertised right now
- A section on what continuous monitoring would add over a one-off report

## How it's built

Python, an LLM for reading flyer images, public search, and automated PDF generation. The
implementation and the methodology are kept private; this repo is just an overview.

## Limits and ground rules

- Public data only. No logins, no scraping behind a sign-in.
- Events, never individuals. No biometrics or facial recognition.
- Not crime prediction, and not meant for evidence.
- The matching is not perfect, so anything low-confidence is flagged instead of stated as fact.

Built by Tracecast LLC.
