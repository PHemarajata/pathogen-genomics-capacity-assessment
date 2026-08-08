# Release notes: Full Baseline v8, Short Form v4 and Enabling Environment Annex v1

APHL Global Health, Pathogen Genomics Capacity Assessment. August 2026.

Supersedes Full Baseline v7 and Short Form v3. Adds the Institutional and National Enabling Environment Annex v1, which is new.

---

## Why this release exists

v7 was standards-driven. It closed gaps against CLSI EP49, MM24 and EP12-A2 and it did that well. v8 is administration-driven. It comes out of running the instrument three times at one site in May 2026 and cataloguing what it could not express, could not compare or made uncomfortable to ask.

Three findings shaped almost everything below.

Yes and no could not hold what the laboratories actually were. A quality system in working-draft form, an automation platform in implementation, a sequencer in place but not running, a policy that exists alongside inconsistent practice. All of that resolved into narrative rather than into data, which meant it could not be counted, compared or tracked.

About a third of what surfaced was not a laboratory finding. Procurement lead times, employment modality, retention policy, multi-year funding and access and benefit sharing all sit above the laboratory. Asked at laboratory level three times, they produced three sets of near-identical recommendations addressed to people who could not act on them.

The instrument counted what a laboratory owned rather than what it could do. Inventory read strong where the sequencing operation was not yet functional and the routine work happened on a neighbouring laboratory's instrument.

---

## Backward compatibility

Storage keys are unchanged in both instruments. A partially completed v7 or v3 assessment open in the same browser will load without migration.

Question keys from v7 and v3 are preserved wherever the question is unchanged. Where a question was replaced, the old key is retired and a new key introduced rather than the old key being reused with a different meaning. This matters for the second assessment round: an answer under a retired key is a v6 or v7 answer and should not be read as a v8 answer to a similar-looking question.

Retired keys, full baseline: `a6_partners`, `e7_util`, `j1_roles`, `j2_training`, `j4_left_12mo`, `j4_left_24mo`, `j4_tracked`, `j4_reasons`, `l1_sources`, `l2_costs`, `h4_schemes`, `h4_last_date`, `h4_last_outcome`, `e9_planned`, `m1_priority_1` through `m1_priority_3`.

Retired keys, short form: `role_N_filled`, `role_N_vacant`, `role_N_planned`, `staff_left`.

A documented v6 to v7 to v8 crosswalk is not in this release. It is needed before results from the next round are compared to May 2026 and it is tracked separately.

---

## Full Baseline v8: what changed

### The response scale

A five-level maturity scale is introduced alongside yes and no. It is not applied everywhere. Physical facts, counts, dates and roster entries stay as they are, because forcing a scale onto a binary lengthens the visit and adds noise.

| Level | Meaning |
|---|---|
| 0 | Not present and not currently planned |
| 1 | Decision taken, work underway, not yet usable |
| 2 | Working in practice but not documented, or documented but not in routine use |
| 3 | Documented and in routine use |
| 4 | As level 3, plus evidence of effectiveness from audit, EQA, competency or monitoring data |

Level 2 is the load-bearing one. It is where most of the first round actually sat.

Each of the eight rated domains now has written level descriptors, visible in the instrument behind the "Level definitions" panels. Without these two assessors rate differently and ratings are not comparable between rounds, which defeats the purpose of having them.

### Two ratings, kept separately

The laboratory self-rates eight domains, in the sections where the underlying work is discussed. The assessor rates the same eight in Section N. Both are kept.

A gap between them is information rather than an error. Where the laboratory rates itself higher it usually means evidence exists that the assessor did not see. Where it rates itself lower it usually means a standard is understood but not yet met. The instrument computes the difference and displays it in Section N and in the summary.

Two further domains are derived rather than rated. Application operational status comes from the assay portfolio, and workforce continuity comes from the function coverage matrix. Neither is self-rated, because asking a laboratory to rate its own continuity produces defensive answers.

### Section by section

**A.1** adds a stage-of-development field, so that findings are read against where the laboratory is. A laboratory a year into build-out and a mature reference laboratory should not read as the same finding at level 1.

**A.6** replaces the four-column partner roster with a six-facet one: organization type, principal flow, channel, instrument, end date and what stops if it ends. A support profile is computed live. The old structure made every laboratory look diversified, because it grouped a multilateral agency supplying bridging reagents, a financing mechanism moving money through government and a university running joint analysis into one category.

**A.8** is new. Specimens received from other laboratories or countries, work sent out for sequencing performed elsewhere, referral agreements, and the size of any network the laboratory coordinates. Sequencing performed by a partner previously read as capability the laboratory held.

**B.1** adds temperature and humidity specification for the library preparation and sequencer rooms, monitoring modality, excursions recorded, and runs lost or deferred to environmental conditions. This was an active constraint on sequencing operations at one laboratory in the first round and nothing asked about it.

**B.2** converts the biosafety manual review question from yes or no to a date plus document reference plus status. It was answered "unsure" at all three laboratories, which told us nothing. A date the respondent cannot supply is a clearer finding than an unsure box, and it is usually a quality officer question rather than a bench question.

**B.4** adds the date the generator was last actually tested alongside the stated test frequency. Policy and practice diverged at every site.

**C.1** de-lumps specimen sources. Public and private referral networks are listed separately because they behave differently on volume, metadata quality and turnaround expectation.

**C.2b** is new. Turnaround measured against seven fixed anchor points in calendar days, with the main driver of delay at each step, plus run frequency, minimum viable batch size and typical wait for a batch to fill. Three laboratories reported against three different clocks and one reported two of its own. Batching was the actual driver at two sites and was never asked about directly.

**C.3** adds the traceability self-rating.

**E.7** replaces the utilisation roster. Each instrument is recorded as owned and in routine use, owned but underutilised or non-functional, accessed at another laboratory, on order or planned, with runs in the past 12 months, the reason for underutilisation and where it is accessed. Runs per instrument per year is the single number that would have surfaced the largest measurement error in the first round.

**E.9** replaces the free-text acquisitions field with a roster carrying funding status: secured, requested and pending approval, unfunded, or under discussion. Items pending approval are exactly what a national-level recommendation should target and were previously visible only if the assessor happened to note them.

**F.10** splits connectivity into three constraints with different remedies: raw bandwidth, institutional policy, and routing or reliability. Adds where the test was run, the provider, the result reference, and whether an exception process exists with institutional IT. All three laboratories reported a blocked genomics workflow while measuring bandwidth well above the level at which that should happen, which means the constraint was policy, not capacity.

**F.11** adds the bioinformatics reproducibility self-rating.

**H.2** keeps the v7 EP49 three-validity questions unchanged and adds self-ratings for quality documentation, SOP currency, validation practice and competency.

**H.4** replaces the EQA scheme checklist with a roster carrying provider type, scope, who pays, last cycle and outcome. A commercial subscription, a WHO network panel and a peer-institute exchange are not the same commitment, and the difference determines what happens when a project ends.

**H.4b** is new. Whether the laboratory provides EQA or proficiency panels to others. This is a capability tier above participation and directly relevant to regional role.

**H.6** is new. The assay portfolio: every assay in scope with platform, intended use, status, standard used and whether clinical validity is documented. This replaces the section-level validation question, which was answered yes at every laboratory while metagenomics sat unvalidated for clinical use. Both statements were true and the old structure could not hold both.

**H.7** is new. A sixteen-point documentation walkthrough across up to three assays, chosen by the laboratory. Framed in the instrument as a walkthrough and not an audit. Not scored, not aggregated, not compared between laboratories.

**I.1** adds utilisation percentage, annual growth and projected time to capacity, and separates the retention policy question into whether a written institutional policy exists at all.

**I.2** adds the date a restore was last tested, where the backup sits, and whether it shares a power supply with the primary. Two laboratories in the first round named a third as their disaster recovery arrangement and all three were on one campus.

**I.4b** is new. Access and benefit sharing as named fields: whether external sharing is constrained, since when, which repositories, how many datasets are held pending release, and the stated resolution pathway. Framed as a policy constraint rather than a capacity gap, because that is what it is.

**J.1** replaces the headcount roster with a twelve-function coverage matrix. For each function: how many can perform it independently, how many of those are under twelve months in role, the employment basis of primary coverage, and what happens on a two-week absence. Single-person dependency is derived rather than asked.

**J.1b** is new. Establishment: authorised and funded, filled, authorised but unfunded, functions performed with no established position, and roles identified as needed but not established. A role the laboratory needs that does not exist on paper is not a vacancy and had nowhere to go before.

**J.2** rebuilds the training roster with provider type, who paid, delivery mode and whether the training is repeatable in-country without the provider. That last column is the one that matters for sustainability.

**J.4** removes the departure-count questions. Retention moves to institutional leadership, where it is a management question rather than an implied judgment on the laboratory. What remains is forward-facing: training investment retained, people trained who are no longer performing NGS functions here, and expected staffing change. The second of these also picks up internal promotion and further study, which are not failures and were previously being read as such.

**K.0** is new. A recipient matrix per application: who receives the result, in what form, in what timeframe, and whether receipt or action is confirmed. The last-mile gap recurred at every laboratory in the first round and sat underneath a stakeholder checklist that produced long lists.

**L.1** retires the funding-source checklist. The funding profile is derived from the partnership roster in A.6 and displayed in L.1, so the same thing is not asked twice at two different levels of resolution. What remains is concentration, domestic share and fee-for-service authority.

**L.2** replaces the cost roster with one carrying basis, currency, assumed batch size, derivation and as-of date. The first round produced a range spanning a factor of four with none of these stated, which made the figures unusable for the fee-for-service conversation one laboratory wanted to have.

**L.3** measures the supply chain rather than describing it. Lead time as shortest, typical and longest. Stockout events and days of operation lost. Whether reagents expired in storage. Count of sole-source critical reagents. And, separately from whether reorder triggers exist, whether they were acted on, with a field for what prevented it. Every laboratory reported documented triggers while one described being unable to set meaningful trigger points because shelf life is shorter than lead time.

**M.1** splits the priorities question three ways: ranked capacity-building topics from a fixed list, support requests that are not training, and requests better directed to partners other than APHL. Two of three laboratories led with something outside MADE scope and one led with procurement support, which is not a training topic at all.

**M.6** adds three prompted narrative questions: a genomic result that changed a decision, an operational failure or near miss, and something the laboratory is proud of that the assessment did not ask about. The richest material in the first round arrived by luck of conversation.

**Section N** is new and is the assessor record, not a laboratory section.

- N.0 assessment record, including instrument version, round, prior assessment date and prior instrument version
- N.1 assessor domain ratings with the written level definitions and the divergence readout
- N.2 evidence basis per section: self-reported, document sighted, observed in operation, or demonstrated
- N.3 findings log, each tagged with the level that can act on it and its evidence basis
- N.4 shared-resource module across ten capabilities: owned, shared, accessed elsewhere, provided centrally or unavailable, plus the arrangement

### Assessment Summary

New view, available at any point from the toolbar. Headline counts, the domain grid with self-rating and derived rows marked, the continuity table, the support profile, instrument utilisation, the assay portfolio and the findings sorted by the level that can act. It prints.

### Export

Rewritten. It now leads with a derived summary and the domain grid, then the findings routed by level, then the full responses. Grids and rosters export with their column labels and subsection headings rather than as raw field keys. A structured file export is not in this release.

### Demo dataset

A "Load demo data" button populates an illustrative composite laboratory. It is not any real laboratory. It exists for training assessors and for demonstration, and it is built to contain the patterns worth discussing.

---

## Short Form v4: what changed

The short form stays light. Target is still about 30 minutes and no maturity ratings, partner taxonomy, procurement detail or validation walkthrough have been added to it.

**2.4** adds an assay portfolio roster, eight rows, minimal fields. This is the largest pre-visit scoping gain: the visit no longer starts by building the list.

**2.5** asks which assays the laboratory would like to walk through during the visit. This seeds H.7 of the baseline and puts the choice with the laboratory before anyone arrives.

**3.4** adds instrument ownership, access and utilisation with runs in the past 12 months.

**3.5** asks what capability is routinely accessed at another laboratory or provided centrally.

**4.1** replaces the headcount-by-role table with a six-function coverage matrix: independent coverage and two-week absence impact. An on-page note explains the change, because respondents who completed v3 will notice.

**4.2** removes the departures count and replaces it with how many of the people trained are still performing NGS functions.

**7.4 and 7.5** split support requests that are not training, and requests better directed to other partners, out of the priorities boxes.

The export carries all the new blocks plus a short derived read on utilisation and continuity.

---

## Enabling Environment Annex v1: new instrument

Administered once per site with institutional leadership, and with ministry participation where it can be arranged. Laboratories do not complete it. Separate storage key, so it can be open alongside the baseline in the same browser.

It exists because about a third of what a laboratory assessment surfaces is not a laboratory finding, and asking those questions of three laboratories on one campus produced three near-identical recommendation sets addressed to people who could not act on them.

**A. Site record.** Institution, laboratories in scope, respondents by role, and which authorities were present. Where budget, establishment, procurement or ministry authority was absent, the sections depending on it are flagged as second hand rather than treated as confirmed. That flag propagates to the summary and the export.

**B. Establishment and employment.** Where the retention conversation now lives. Employment modality by function rather than headcount, whether an approved position description exists, the route to create an established post and how long it takes, salary competitiveness, career ceiling for technical staff, and turnover with fixed departure reasons. Internal promotion and further study are options because they are frequently the largest category and are not failures.

**C. Procurement.** A seven-step decision grid recording who decides at each step, duration and variability. The count of separate approvals is usually a better predictor of lead time than any single step, and variability rather than length is what makes planning impossible. Plus expedited and sole-source routes, whether shelf life is considered in scheduling, and what would have to change for lead times to halve.

**D. Budget and funding cycle.** Fiscal year and confirmation timing, multi-year commitment mechanisms, domestic against external share, whether a transition mechanism exists and has ever been used, and where cost-recovery revenue goes.

**E. Data governance.** Retention policy and whether it addresses genomic data, cloud and off-site position, who authorises external transfer and how long it takes, and whether standing authorisation is possible for routine surveillance.

**F. Access and benefit sharing.** Status, scope, stage, repositories affected, backlog, oldest dataset held, who owns the resolution and confidence in the timeline.

**G. National strategy and coordination.** Strategy, funded implementation plan, coordinating body and whether it meets and decides, network tiering, known duplication, and which external commitments current capacity does not meet.

**H. Shared infrastructure and continuity.** Twelve centrally provided services by provision, owner and service level. Sharing between laboratories. And whether any laboratory's disaster recovery depends on another laboratory on the same campus and power supply.

**I. Accreditation and regulatory.** Licensing, ISO 15189 scope and whether sequencing is in it, institutional quality resourcing, and whether a national pathway for laboratory-developed tests exists at all. That last one is frequently unknown at laboratory level and determines what a laboratory must demonstrate before reporting a sequencing assay clinically.

**J. Assessor synthesis.** Six enabling-environment domains, E1 to E6, with written level anchors and a leadership self-rating alongside the assessor rating. Evidence basis per section. A findings log where every row carries the level, **who specifically can decide**, the next step and the laboratories affected. A finding routed to "the ministry" is not actionable; one routed to a named role with a next step is. And a written paragraph for the site synthesis on what the laboratories cannot fix, which is the passage laboratory leadership can quote upward.

**Laboratory confirmation extract.** A separate view generating one printable page per laboratory, listing only the findings that bear on it with agree and comment boxes and a signature line. This is how laboratories stay in the record without being asked the same questions a third time. Findings tagged "All" appear on every extract; findings naming particular laboratories appear only on theirs.

**Verification.** Renders ten sections with no runtime errors, no leakage of baseline-specific content, distinct storage key, and clean runs of demo load, summary, extract generation, divergence computation, persistence and export.

**Fixed before release, and confirmed in a real browser.** The first annex build inherited `updateModuleVisibility()` from the baseline, which drives the Section G application modules. The annex has no modules, so the function threw on a missing element during start-up. Because it was called part-way through `initApp()`, everything after it was skipped: the auto-save listeners never attached, so nothing was saved; panels did not close on Escape; and derived readouts did not compute on load. The sections themselves rendered, which is why it was not obvious.

Two changes were made in response. The module logic is now a no-op in the annex and null-guarded in the baseline. More usefully, start-up in both instruments is now a sequence of independently guarded steps, so a failure in one is logged to the console and recorded on `window.__initErrors` without preventing the others. Losing a derived readout is recoverable; losing the auto-save listener is not, and the two should not share a failure mode.

---

## What is not in this release

These were approved and are deliberately out of scope for the two instruments.

**Site synthesis report template.** The report layer that holds institutional, national, shared-infrastructure and cross-cutting findings once per site, so that per-laboratory reports reference it rather than restating it.

**Domain Maturity Summary document.** The instrument computes and displays the ratings. The separate internal document with change-since-prior-round and the network-level narrative does not exist yet. Distribution needs deciding before it does.

**Version crosswalk and repeat-assessment mode.** Needed before October results are compared to May.

**Assessor guidance.** Section time estimates, the respondent map by section, and the written framing for the validation walkthrough and the workforce section. Two of these are printed in the instrument as hints; the briefing document is not written.

**Structured gaps export.** The summary renders and prints. A machine-readable export does not exist.

---

## A note on the wrapper's error banner

The standalone wrapper appends a red error panel to the page on the first JavaScript error and leaves it there. It never clears, and subsequent errors are appended to it. This matters when reading a bug report: an error raised during page load stays on screen through everything the user does afterwards, so it can appear to have been caused by whatever they clicked next.

That is exactly what happened with the first annex build. The failure occurred once, during start-up, in code inherited from the Full Baseline. Clicking Load demo data raised nothing at all. Driving the pre-fix build through headless Chromium confirmed both points: the stack shows `updateModuleVisibility` called from `initApp`, and the demo click produces no new console output while the banner text stays exactly as it was.

The practical lesson is that the banner shows the first error, not the most recent action.

---

## Build identification and error reporting

Every instrument now carries a build stamp. It appears in the page footer, in the hero panel, and on `window.__BUILD` in the console, which logs the instrument, version and build on load. If a problem is reported, the first thing to establish is which build was open.

Each instrument also installs its own error handler. The standalone wrapper catches window errors and prints them prefixed with `[bundle]`, reporting the wrapper's own line number rather than the instrument's, which makes them impossible to trace. The new handler logs the real message, source file, line and stack to the browser console. A `[bundle]` line on its own is not diagnostic; the console entry beneath it is.

Current builds are Full Baseline v8.1, Short Form v4.1 and Enabling Environment Annex v1.1, all build 2026-08-08b. Filenames carry the version so a new download cannot be confused with an earlier one sitting in the same folder.

---

## Notes for assessors

**Section N is yours.** Do not hand the instrument to a laboratory with Section N visible as something to complete. If the laboratory sees the findings log mid-visit it changes what they tell you.

**Say the framing out loud, not just in the instrument.** Two sections carry printed framing that matters: the validation walkthrough is a documentation walkthrough and not an audit, and the workforce section is about continuity and not performance. Both were written because of how the first round felt, not only because of what it produced.

**A capability accessed elsewhere is not absent.** Record it as accessed. Coding it as a gap understates the site and manufactures a finding that belongs to nobody.

**Tag the constraint level as you collect.** Reconstructing it during report writing is slower and less accurate than a two-second selection in the room.

**Watch the self-rating divergence before close-out.** Where the laboratory and the assessor disagree by more than one level, that is a conversation to have on site rather than a discrepancy to resolve afterwards.

**The maturity ratings do not go in the partner-facing report.** No total score, no ranking between laboratories, and no comparison across laboratories with different mandates or stages of development.

---

## Verification

All three instruments were checked programmatically and in a headless DOM before release.

Full Baseline v8: renders 15 sections with no runtime errors; all new components present; all superseded fields confirmed absent; v7 EP49 splits and Section G module gating preserved and gating verified to respond to Section A.4; demo load, summary generation, self-rating divergence, state persistence and text export all clean; export confirmed free of raw field keys.

Short Form v4: all new blocks build; v3 application table, yes-no blocks and EP49 clinical validation question preserved; retired fields confirmed absent; new fields persist to storage; progress tracking extended and computing; export carries the new blocks and retains all v3 sections.

Both re-embedded in their original standalone wrappers with fonts and APHL assets intact, and the wrapper bootstrap scripts verified byte-identical to v7 and v3.

A separate init-integrity harness now runs against the shipped standalone files rather than the sources, and checks each instrument in the state it reaches after a natural page load: no uncaught errors, no failed start-up steps, every `getElementById` target present in the DOM, and, most importantly, that typing into a field actually persists to storage. All three pass. This check exists because the annex defect described above was invisible to the functional tests, which called each function by hand and so never observed that start-up had aborted.

All three instruments have also been driven through headless Chromium: page load, demo dataset, summary generation and, for the annex, the laboratory extract. No console errors, no page errors, no failed start-up steps in any of them. This is the check that should have been run before the annex shipped, and it is now part of the release procedure.

Two dead controls were removed while doing this. "Expand all" and "Collapse all" called no-op stubs left over from an earlier collapsible design and did nothing in either instrument.

None of the three instruments has been pilot-tested with a live respondent. That is the remaining check before the next visit.
