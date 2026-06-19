<div align="center">

# WatchTower

**Open-source early warning for publicly-advertised mass-gathering events.**

A product by Tracecast LLC · OSINT for public-safety situational awareness

<img src="docs/cover.png" alt="WatchTower OSINT assessment cover" width="520">

</div>

---

## What it is

Some public-safety incidents are advertised in the open before they happen. WatchTower
surfaces and structures that **public advertising** from open-source signals, then produces a
clean intelligence brief: distinct events, where each was advertised, how strongly it is
corroborated across independent public sources, and a confidence level for each.

It is **detection of public advertising, not prediction of crime,** and it reports **events,
never individuals.**

## What it produces

A multi-section OSINT assessment (PDF):

- **Key judgments** and at-a-glance metrics
- **Pattern analysis** (activity over time, by location, by outcome, by venue type)
- An **event log** with corroboration counts and per-row confidence
- **Flyer extraction** read directly from public images
- A live **on-demand scan** of what is being advertised now
- **Forward capability** — what continuous, live early warning delivers
- Stated **collection method, constraints, and handling rules**

## Operating guardrails

WatchTower is built to be defensible by design:

- **Public, logged-out sources only** — no authentication, no fake accounts
- **No facial recognition, no biometrics — ever**
- **Events, not individuals**
- Links back to public sources; **minimal retention**
- **Not** predictive policing, and **not** evidentiary
- Context classification separates genuine signals from benign look-alikes, with a
  confidence level; low-confidence items are flagged, not asserted

## Tech

Python · large-language-model vision for image understanding · open-source search ·
automated report generation.

## Status

Working prototype. This is a real, privately-developed product; the implementation and
methodology are kept private. This repository is a public overview of the project.

---

<div align="center">
<sub>WatchTower · Tracecast LLC · Open-source · public data only</sub>
</div>
