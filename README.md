# Lakehouse Blueprints

**An interactive reference-architecture composer for the Databricks Lakehouse.**
Live at **https://jason-miles.github.io/lakehouse-blueprints/**

Pick a scenario — Streaming ETL, Fraud & AML, GenAI Assistant, BI & Analytics,
or ML at Scale — and the page composes a tailored architecture: the medallion
flow (Sources → Ingest → Bronze → Silver → Gold → Serve), the specific
Databricks components, a bill of materials, and design notes. Click any
component to see what it does. Unity Catalog governance spans every layer.

Built as a conversation starter for architecture discussions — a fast, visual
way to show *shape* before diving into a detailed design.

## Design

A single self-contained `index.html` — no build step, no framework. Space
Grotesk, a near-black / warm-paper canvas that follows the visitor's light/dark
preference, one Databricks-red accent. Shares the design language of
[jason-miles.github.io](https://jason-miles.github.io).

```
index.html            # the whole app (inline CSS + vanilla JS, data-driven)
assets/favicon.svg    # brand mark
assets/og-card.png    # social share image
```

Scenarios and components live in the `SCENARIOS` / `C` objects in `index.html` —
edit those to add or adjust patterns.

## Note

These are **illustrative reference patterns** — a starting point for
architecture conversations, not an official Databricks reference or pricing.
