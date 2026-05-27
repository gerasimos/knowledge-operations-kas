# Changelog

All notable changes to this work are documented in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
This is a living document; versions increment when content changes meaningfully.

- **Patch** (`0.1.x`) — typo fixes, broken links, citation metadata corrections, formatting.
- **Minor** (`0.x.0`) — new sections, expanded examples, additional citations, new appendices, new figures.
- **Major** (`x.0.0`) — thesis revisions, framework restructuring, removal or renaming of named concepts (K0–K6, G0–G5).

Each release is archived to Zenodo with its own version-DOI; the concept-DOI [10.5281/zenodo.20083456](https://doi.org/10.5281/zenodo.20083456) always resolves to the latest archived version.

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
