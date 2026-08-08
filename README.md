# Pathogen Genomics Capacity Assessment

**A field-tested instrument set for assessing pathogen genomics laboratory capacity, built for reuse.**

Developed by APHL Global Health under the MADE Initiative. First deployed across three laboratories at the Research Institute for Tropical Medicine (Manila, Philippines) in May 2026; revised into the current release from what that round exposed.

---

## What this is

A structured assessment system for pathogen genomics (NGS) laboratory capacity, delivered as three self-contained HTML instruments:

| Instrument | Version | When it's used | Respondent | Time |
|---|---|---|---|---|
| [**Short Form**](instruments/NGS_Assessment_Short_Form_-_APHL_v4.1__standalone_.html) | v4.1 | Sent 2–3 weeks ahead of a visit, to scope it | One senior respondent per laboratory | ~30 min |
| [**Full Baseline**](instruments/NGS_Assessment_Full_Baseline_-_APHL_v8.1__standalone_.html) | v8.1 | On site, over 1–2 days | Laboratory team, with assessor | 1–2 days |
| [**Enabling Environment Annex**](instruments/NGS_Assessment_Leadership_Annex_-_APHL_v1.1__standalone_.html) | v1.1 | Once per site, with institutional leadership | Leadership (ministry participation where possible) | Half day |

Each instrument is a single HTML file. **No server, no subscription, no internet connection, no installation.** They run in any modern browser — including on a tablet at the bench — auto-save locally as you type, and export structured data.

## Getting started

1. Download the instrument you need from [`instruments/`](instruments/) (open the file, then use the **Download raw file** button — or grab everything via **Code → Download ZIP**).
2. Open the file in a browser. It works fully offline.
3. Use **Load demo data** to populate an illustrative composite laboratory — built for assessor training and demonstration, containing the patterns worth discussing. It is not any real laboratory.
4. Responses persist in the browser between sessions. The **Assessment Summary** view (toolbar) and the text export are available at any point.

Each instrument carries a build stamp — in the page footer, in the hero panel, and on `window.__BUILD` in the browser console. Current builds are Full Baseline v8.1, Short Form v4.1, and Enabling Environment Annex v1.1, all build **2026-08-08b**. If you report a problem, start by identifying which build was open.

## What makes it different

**It routes every finding to the level that can act on it.** Roughly a third of what a laboratory assessment surfaces is not a laboratory problem — procurement lead times, employment modality, data retention policy, multi-year funding. Every finding carries a constraint-level tag (laboratory / institution / above the institution), and reports are structured the same way, so the national-level section can be quoted directly by laboratory leadership in upward communication.

**It measures continuity, not headcount.** For each of twelve laboratory functions: how many people can perform it independently, and what happens if the usual person is unavailable for two weeks. Single-point-of-failure exposure falls out of the answers rather than being asked about directly.

**It distinguishes what partners actually provide.** Each partnership is recorded across what flows (cash, in-kind reagents, equipment, technical assistance, sequencing performed by the partner), through what channel, under what instrument, ending when, and what stops if it ends — yielding funding concentration, cash/in-kind splits, an expiry calendar, and a map of single-point dependencies.

**It is anchored to clinical laboratory standards.** Questions are built against ISO 15189:2022 and relevant CLSI guidance — EP49 (clinical validity), MM24 (bacterial WGS and strain typing), EP12-A2 (qualitative test performance). Validation status is captured per assay, not per laboratory, and analytical validation is separated from clinical validation.

**It produces two outputs for two audiences, without conflating them.** A narrative report for the laboratory and its partners, and a separate internal domain-maturity summary for program management. No total score, no ranking between laboratories — deliberately, because an instrument that produces a score a laboratory can be judged on changes what laboratories tell you.

## The maturity scale

A five-level scale is applied to a defined subset of questions (physical facts, counts, and dates stay binary or numeric):

| Level | Meaning |
|---|---|
| 0 | Not present and not currently planned |
| 1 | Decision taken, work underway, not yet usable |
| 2 | Working in practice but not documented, or documented but not in routine use |
| 3 | Documented and in routine use |
| 4 | As level 3, plus evidence of effectiveness from audit, EQA, competency or monitoring data |

The laboratory self-rates eight domains; the assessor rates the same eight independently. Both are kept, and the divergence is computed and displayed — a gap is information, not an error.

## Why it transfers

Nothing in the laboratory instruments is country-specific. Application modules select automatically based on the sequencing work a laboratory actually performs, so the same instrument serves a viral surveillance laboratory, a bacterial AMR reference laboratory, and a laboratory in its first year of build-out. Country-specific policy context lives in the Enabling Environment Annex — which is what makes multi-country use possible: the laboratory instrument stays constant (findings comparable across countries) while the annex absorbs the regulatory, procurement, and employment contexts that differ everywhere.

A new country deployment requires: assessor familiarization (about half a day), 2–3 days on site for a three-laboratory site, access to institutional leadership for the annex, and local adaptation limited to the annex and regulatory references.

## Repository contents

```
instruments/
  NGS_Assessment_Short_Form_-_APHL_v4.1__standalone_.html      Pre-visit scoping form
  NGS_Assessment_Full_Baseline_-_APHL_v8.1__standalone_.html   On-site baseline assessment
  NGS_Assessment_Leadership_Annex_-_APHL_v1.1__standalone_.html Enabling environment annex
docs/
  pathogen-genomics-assessment-brief.md / .pdf                 Two-page overview of the system
  release-notes-v8-v4-2026-08.md / .pdf                        Full release notes for the current builds
CHANGELOG.md                                                   Version history at a glance
```

Filenames carry the version so a new download cannot be confused with an earlier one sitting in the same folder.

## Version notes

Current release: **Full Baseline v8 / Short Form v4 / Annex v1** (August 2026), superseding Full Baseline v7 and Short Form v3. The full story of what changed and why is in the [release notes](docs/release-notes-v8-v4-2026-08.md); the short version is that v7 was standards-driven and v8 is administration-driven — built from cataloguing what three real administrations of the instrument could not express, could not compare, or made uncomfortable to ask.

Backward compatibility: storage keys are unchanged, so a partially completed v7/v3 assessment open in the same browser loads without migration. Question keys are preserved where the question is unchanged; replaced questions retire the old key rather than reusing it with a different meaning. The retired-key lists are in the release notes.

## Status and roadmap

The current builds are verified programmatically, in a headless DOM, and through headless Chromium (page load, demo data, summary generation, annex extract — no console errors, no failed start-up steps). They have **not yet been pilot-tested with a live respondent**; that is the remaining check before the next visit.

Planned for the next cycle (target: Q4 2026): a version crosswalk and repeat-assessment mode (needed before October results are compared to May), the site synthesis report template, the domain maturity summary document, the assessor briefing document, and a machine-readable gaps export.

## Notes for assessors

The instruments embed key framing, but four points bear repeating: Section N of the Full Baseline is the assessor's record and should not be visible to the laboratory mid-visit; the validation walkthrough is a documentation walkthrough, not an audit — say so out loud; a capability accessed at another laboratory is recorded as *accessed*, not absent; and maturity ratings do not go in the partner-facing report.

## Attribution

APHL Global Health, Southeast Asia. Pathogen Genomics Capacity Assessment, 2026. Developed under the MADE Initiative.

## License

No license has been applied yet; all rights reserved. If you are interested in using or adapting the instruments, please open an issue or get in touch.
