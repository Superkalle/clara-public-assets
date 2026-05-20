# CLARA · Executive Asset Hub

Public distribution repository for CLARA executive assets — onepagers, boardroom decks, whitepapers, partner kits, workshop briefings and thought leadership.

Site:

```text
https://superkalle.github.io/clara-public-assets/
```

Custom domain target (when configured):

```text
https://assets.decisiongovernance.de/
```

---

## Languages

The hub is bilingual.

- German (default) at `/`
- English at `/en/`

Every asset in this repository is published with `-de` (German, primary) and unsuffixed (English) variants where rendered.

---

## What this repository is

This is the public distribution layer of the CLARA Executive Communication Operating System.

It exists to make CLARA's executive assets directly shareable as PDFs, HTML files and static URLs — without exposing the positioning, sales or generation infrastructure that produces them.

The source of truth for the assets themselves lives in a separate, non-public positioning repository.

This repository receives:

- approved executive artifacts
- the asset hub landing pages (DE + EN)
- the GitHub Pages deployment workflow

It does not contain:

- positioning sources
- sales mechanics
- generation prompts
- internal operational documentation

---

## CLARA

CLARA is the governance and decision layer between discussion and execution.

CLARA is positioned as:

- a Decision Governance Platform
- a Decision Intelligence Layer
- a structured layer between communication and execution
- an Organizational Clarity System
- a Decision Hygiene system for AI-accelerated organizations

CLARA is not positioned as:

- a chatbot
- a generic AI assistant
- an autonomous AI decision engine
- a workflow or reporting tool
- a productivity app or prompt wrapper

---

## Repository layout

```text
index.html               DE asset hub (default entry point)
en/index.html            EN asset hub
onepager/                executive onepagers (DE + EN variants)
board-decks/             boardroom-level executive decks (DE + EN variants)
whitepapers/             decision governance / decision hygiene papers
partner-kits/            externally shareable partner enablement bundles
workshop-assets/         workshop briefings and supporting materials
linkedin-assets/         thought leadership visuals
```

Every category folder contains its own README describing the category, the current published version and the intended audience.

---

## Versioning

Every asset carries an explicit version suffix:

```text
CLARA-Executive-Onepager-v2-de.pdf   (German, primary)
CLARA-Executive-Onepager-v2.pdf      (English)
CLARA-Boardroom-Deck-v1-de.pdf
CLARA-Boardroom-Deck-v1.pdf
```

Versioning rules:

- `vN` is incremented when the asset is materially regenerated.
- A `v(N+1)` supersedes prior versions. Older versions move to `archive/` inside the category folder.
- The version in the file name matches the version line printed inside the asset.
- German is the primary distribution language; English variants are produced alongside.

`archive/` folders are retained in the repository for traceability but excluded from the deployed Pages site.

---

## External sharing

Public assets may be shared with:

- prospective pilot customers
- executive contacts at qualified organizations
- partners and multipliers operating under explicit positioning alignment
- boards, investors and advisory contexts
- public LinkedIn and executive channels

Every asset reinforces the same positioning. Differences between assets are differences of audience and depth — not of message.

---

## Deployment

The asset hub is published via GitHub Pages.

- Workflow: `.github/workflows/deploy-assets.yml`
- Trigger: push to `main`
- Build: stages the repository root into `_site/`, excluding `.git`, `.github` and any `archive/` subdirectories
- Entry point: `index.html`

The workflow refuses to deploy if the entry point is missing.

---

## Quality

Every asset published here has passed an internal quality review for:

- executive tone
- governance positioning consistency
- anti-hype compliance
- visual consistency with the cockpit4me design system
- boardroom readability
- procurement compatibility
- category discipline
- naming and versioning
- source coupling
- promotion hygiene

Assets that do not satisfy these conditions are not published here.

---

## Executive statement

Organizations do not fail because they lack information.

Organizations fail because decisions become unclear under pressure.

CLARA exists to stabilize governance, clarity and decision quality in increasingly complex environments.
