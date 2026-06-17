# Changelog

All notable changes to this work are documented in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
This is a living document; versions increment when content changes meaningfully.

- **Patch** (`0.1.x`) — typo fixes, broken links, citation metadata corrections, formatting.
- **Minor** (`0.x.0`) — new sections, expanded examples, additional citations, new appendices, new figures.
- **Major** (`x.0.0`) — thesis revisions, framework restructuring, removal or renaming of named concepts (K0–K6, G0–G5).

Each release is archived to Zenodo with its own version-DOI; the concept-DOI [10.5281/zenodo.20083455](https://doi.org/10.5281/zenodo.20083455) always resolves to the latest archived version.

---

## [Unreleased] — 2026-06-17

### Fixed

- Citation metadata now cites the concept DOI `10.5281/zenodo.20083455` (all-versions; resolves to the latest) across the banner, `CITATION.cff`, and this changelog. The v0.1.0 deposit's version-DOI `10.5281/zenodo.20083456` is retained only where that specific release is referenced.
- Stripped build/template and figure-construction comments from the published `index.html` (they exposed the pandoc pipeline and SVG internals in page source).

---

## [v0.2.0] — 2026-06-16

Maintenance revision.

### Added

- Appendix D: kill criteria (conditions for retiring or revising the framework).
- §13.1: worked example of the capability-profile template, plus an operational-signature table (latency, cost, reliability) and a knowledge-preparation prerequisite.
- OKF (Open Knowledge Format) positioned as a layer-1 substrate standard: Appendix C.2 mapping, §4.2 citation, a §10 anti-pattern, a §12.3 checklist question, references [32]–[33].
- §8.1: a result-completeness signal for predicate-countable stores (report qualifying-set size; flag truncation).

### Changed

- Appendix C renamed to "Relationship to external standards" (C.1 OASF, C.2 OKF).
- K1 defined as scoping by typed predicate; permission enforcement is the G2 control-plane case, not the operation.
- K2 defined as structure-scoped query in, structurally-attributed result out, with parent/sibling neighborhood.
- §8.2 K6 artifacts: counterfactual plan-variance and recovery probes replace fixed expected tool-call sequences.
- Governance presented as named bundles, not a cumulative staircase; operation-verb vocabulary aligned across sections.

### Fixed

- §14 reference to a non-existent "kill-criteria appendix" (now Appendix D).
- Figure labels: K1 operation "Filter" → "Scope"; §12.3 figure updated to 10 questions.
- OASF mappings re-pinned to v1.0.0; duplicate passages trimmed; minor terminology and metadata corrections.

---

## [v0.1.0] — 2026-05-21

### Initial public release

First public release of the framework as a living document on GitHub Pages.

The whitepaper defines **Knowledge-Augmented Systems (KAS)** as AI systems that combine language models with external knowledge, structure, computation, and execution. It introduces:

- A **knowledge-operations** vocabulary (retrieve, scope, interpret, combine, compute, traverse, orchestrate, govern, evaluate) as the unit of capability analysis.
- Seven capability **archetypes** (K0–K6) — workload-shape labels, deliberately not a maturity ladder.
- A six-level **governance scale** (G0–G5) applied across operations.
- A per-class **evaluation discipline** including abstention and calibrated uncertainty as first-class system properties.
- A **prescriptive floor** — three explicit conditions under which a capability profile is insufficient, so the framework retains prescriptive force without collapsing into "fitness to task" relativism.
- **15 sections + 3 appendices**, 18 figures, 31 primary citations.

Archived to Zenodo: [10.5281/zenodo.20083456](https://doi.org/10.5281/zenodo.20083456).

### Repository publishing rollout

v0.1.0 is being populated into the public GitHub repository in incremental commits over a few sessions, rather than as a single bulk import. The paper content (text, figures, citations) is unchanged across these commits — only the repository-level files (LICENSE, README, CSS, build pipeline, contributor scaffolding) accumulate. No version bump applies to these rollout commits.

Rollout log (most recent first):

- 2026-05-27 — `assets/whitepaper.css` added so the GitHub Pages render at <https://gerasimos.github.io/knowledge-operations-kas/> displays with its intended typography and sidebar TOC layout. (The initial commit shipped `index.html` referencing this CSS file but omitted the file itself.)
- 2026-05-27 — Initial commit: `LICENSE`, `CITATION.cff`, `README.md`, `index.html`, `.gitignore`.
