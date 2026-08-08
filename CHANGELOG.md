# Changelog

Full detail for every release lives in [docs/release-notes-v8-v4-2026-08.md](docs/release-notes-v8-v4-2026-08.md).

## Build 2026-08-08b — August 2026

**Full Baseline v8.1 · Short Form v4.1 · Enabling Environment Annex v1.1**

- **v8.1 / v4.1 / v1.1 (patch):** Annex start-up defect fixed — an inherited `updateModuleVisibility()` call aborted `initApp()` mid-sequence, silently disabling auto-save. Start-up in all instruments is now a sequence of independently guarded steps; failures are logged to console and `window.__initErrors`. Build stamps added (footer, hero panel, `window.__BUILD`). Per-instrument error handlers report real file/line/stack instead of opaque `[bundle]` lines. Dead "Expand all"/"Collapse all" controls removed. Init-integrity harness and headless Chromium checks added to the release procedure.

## Full Baseline v8 — August 2026

Administration-driven revision from the May 2026 round at RITM Manila. Highlights:

- Five-level maturity scale with written level descriptors on a defined subset; laboratory self-rating and independent assessor rating with computed divergence
- Six-facet partnership roster (A.6) with live support profile; inter-laboratory flows (A.8, new)
- Turnaround against seven fixed anchor points with batching questions (C.2b, new)
- Instrument utilisation with runs per platform per year, replacing inventory counts (E.7); acquisitions roster with funding status (E.9)
- Connectivity split into bandwidth vs. policy vs. reliability constraints (F.10)
- Per-assay portfolio with validation status (H.6, new), replacing section-level validation questions; sixteen-point documentation walkthrough (H.7, new); EQA roster with provider type and payer (H.4); EQA provision to others (H.4b, new)
- Twelve-function workforce coverage matrix replacing headcount roster (J.1); establishment mapping (J.1b, new); departure counts removed, retention moved to institutional leadership (J.4)
- Reporting recipient matrix per application (K.0, new) — the last-mile gap
- Funding profile derived from the partnership roster (L.1); cost roster with basis, currency and derivation (L.2); measured supply chain — lead times, stockouts, sole-source counts (L.3)
- Section N (new): assessor record — domain ratings, evidence basis, findings log tagged by the level that can act, shared-resource module
- Assessment Summary view; rewritten export leading with derived summary; demo dataset

## Short Form v4 — August 2026

Stays at ~30 minutes; no maturity ratings added. Adds an eight-row assay portfolio roster (2.4), walkthrough assay selection to seed the visit (2.5), instrument ownership/access/utilisation (3.4), capabilities accessed elsewhere (3.5), a six-function coverage matrix replacing the headcount table (4.1), and split support-request questions (7.4/7.5).

## Enabling Environment Annex v1 — August 2026 (new instrument)

Administered once per site with institutional leadership. Ten sections covering establishment and employment, procurement decision grid, budget cycle, data governance, access and benefit sharing, national strategy, shared infrastructure and continuity, accreditation and regulatory pathway, and assessor synthesis with findings routed to named decision roles. Generates a one-page confirmation extract per laboratory.

## Earlier

- **Full Baseline v7 / Short Form v3** — standards-driven revision closing gaps against CLSI EP49, MM24, and EP12-A2. Superseded by v8/v4.
