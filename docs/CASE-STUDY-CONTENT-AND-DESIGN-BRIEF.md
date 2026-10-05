# Autonomous Trading Systems Lab public case study — content and design brief

## Purpose

This document is the maintenance source for the public-facing Autonomous Trading Systems Lab
case study. It preserves the audience strategy, claim boundaries, page
structure, visual system, and refresh process so future edits do not drift into
either vague portfolio language or overstated engineering claims.

The case study should help a recruiter, founder, executive, hiring manager, or
technical reviewer understand three things quickly:

1. what problem Chien took responsibility for;
2. how the system and AI-assisted operating model were architected; and
3. why that work is relevant to AI implementation and technical solutions roles.

The case study is not a trading product pitch. The domain creates a useful
high-consequence setting for demonstrating implementation judgment.

## Audience hierarchy

| Audience | Time available | Question to answer | Primary surface |
| --- | ---: | --- | --- |
| Recruiter | 30–60 seconds | Is this person relevant to an AI implementation role? | Hero, executive scan, employer relevance |
| Founder / executive | 2–4 minutes | Can this person turn ambiguity into governed delivery? | Problem, architecture, implementation method, current truth |
| Hiring manager | 5–8 minutes | What did Chien own, and what evidence supports it? | Ownership matrix, failures, proof states, evidence paths |
| Technical reviewer | 10+ minutes | Are the architecture and validation claims internally coherent? | Full markdown, walkthrough, gates, attribution |

## Core positioning

Use this sentence as the canonical positioning idea:

> Chien turns ambiguous, high-consequence workflows into governed,
> testable AI-assisted systems while keeping data quality, decision rights,
> validation, and human accountability explicit.

The central hiring signal is **implementation leadership around AI**, not model
novelty and not trading performance.

### Target role families

- AI Implementation Specialist / Consultant
- Technical Solutions / Solutions Engineer
- AI Operations / Workflow Automation
- Implementation and Onboarding
- Product or Technical Support with AI systems ownership
- Product Operations / Technical Program coordination

## Public narrative architecture

The landing page should keep this sequence:

```text
outcome-led hero
→ 60-second executive scan
→ plain-English problem
→ authority and system architecture
→ implementation operating model
→ failures converted into controls
→ current truth and proof boundary
→ employer relevance
→ deeper evidence paths
→ contact
```

Each section must add a new decision-useful idea. Avoid repeated slogans,
decorative feature lists, or technical detail that does not improve trust.

## Canonical message hierarchy

### Level 1 — what a recruiter should remember

- Chien can structure ambiguous AI implementation work.
- He coordinates AI tools without outsourcing judgment.
- He validates expected versus actual behavior.
- He makes ownership, evidence, and human approval visible.
- He communicates complex systems in plain English.

### Level 2 — what an executive should understand

- The system separates intelligence from authority.
- Deterministic code owns facts, risk, audit, and future execution decisions.
- Models can explain, classify, challenge, and propose; they cannot authorize.
- Delivery happens in small, inspectable slices with explicit stop conditions.
- Failure is converted into reusable controls rather than hidden.

### Level 3 — what a technical reviewer can inspect

- exact-commit review and status separation;
- fail-closed schemas and unknown-state handling;
- provenance and freshness before interpretation;
- append-only audit and durable recovery;
- adversarial testing of evidence judges;
- commit-before-reveal evaluation design;
- human live-readiness gate.

## Claim and evidence policy

### Allowed public claims

- Phases 0–4 are complete at their stated bounded versions.
- Phase 5 is in progress on a private draft branch.
- Protected `main` still has a fail-closed RiskKernel stub at the 2026-10-04
  snapshot.
- Draft PR #176 contains independently accepted slices and active corrections.
- The authoritative lab CI was green at the current October 4 snapshot.
- No language model has runtime authority over risk or execution.
- No `ALLOW` path, live brokerage execution, or positive expectancy is claimed.
- Chien owns framing, product/architecture decisions, tool routing, acceptance
  criteria, evidence review, privacy boundaries, and final promotion.

### Claims that require a new source reconciliation

- a phase moving from in progress to complete;
- PR #176 becoming merge-ready or merging;
- any operator-verified end-to-end result;
- any change to the no-`ALLOW` boundary;
- performance, reliability, uptime, profitability, or business-impact numbers;
- a new live or production environment;
- a new collaborator role or ownership statement.

### Claims prohibited without direct public-safe evidence

- profitable trading or positive expectancy;
- production autonomous trading;
- enterprise financial, banking, regulatory, or compliance implementation;
- AI making final trade or release decisions;
- private collaborator, account, credential, or operational details;
- strategy thresholds, triggers, or proprietary edge logic.

## Source-of-truth order for updates

Never refresh the public page from memory. Check sources in this order:

1. private source repository `AGENTS.md`;
2. `docs/products/autonomous-lab/operations/NOW.md` on protected `main`;
3. the active Phase 5 branch version of `NOW.md`;
4. `GAP-MATRIX.md` and `BUILD-REPORT.md` on the active branch;
5. live GitHub issue and pull-request state;
6. authoritative CI checks on the exact current head;
7. public case-study files for consistency.

If these sources disagree, publish the most conservative supported state and
state the branch boundary explicitly.

## Visual direction

### Thesis

**Technical field report with an executive reading layer.** The design should
feel rigorous, calm, and contemporary—closer to a well-edited systems dossier
than a startup marketing template or a trading dashboard.

### Palette

- near-black green canvas: `#08110f`
- elevated surfaces: `#0c1714`, `#12201c`
- primary ink: `#eef8f2`
- secondary ink: `#b8c9c0`
- signal green: `#a6ffcb`
- review amber: `#f5c66a`
- boundary red: `#ff9c91`
- human-gate blue: `#9dc7ff`

Green means an evidenced or deterministic path, amber means review or active
work, red marks a prohibited boundary, and blue marks human authority. Do not
use status color decoratively.

### Typography

- `Newsreader` for large editorial claims and section headings;
- `Manrope` for plain-language body copy and actions;
- `DM Mono` for status, evidence, architecture labels, and metadata.

The serif creates humanity and editorial confidence; the sans keeps the prose
direct; the mono communicates system state without turning the page into a
terminal theme.

### Layout principles

- Desktop: wide editorial composition with asymmetrical grids.
- Mobile: single-column reading flow with zero horizontal page overflow.
- First viewport: outcome, ownership signal, status, and authority map.
- One memorable visual system: the deterministic-spine / shadow-model boundary.
- Prefer structured HTML/CSS diagrams over invented product screenshots.
- Keep body copy at 16px or larger and interactive labels at 14px or larger.
- Preserve keyboard focus, reduced-motion behavior, semantic headings, and print
  styles.

## Repository surface strategy

| Surface | Job | Maintenance rule |
| --- | --- | --- |
| `index.html` | Recruiter/executive visual landing page | Outcome first; plain English; current bounded status |
| `README.md` | GitHub repository front door | Short positioning, current truth, ownership, reading routes |
| `PUBLIC-CASE-STUDY.md` | Deep narrative | Engineering detail, failures, status matrix, selected evidence |
| `IMPLEMENTATION-WALKTHROUGH.md` | Transferable method | Keep generic enough to apply beyond trading |
| `VALIDATION-AND-RISK-GATES.md` | Trust model | Keep gates, evidence, and fail-closed rules explicit |
| `ATTRIBUTION-AND-LIMITATIONS.md` | Accountability | Update when tool roles or ownership facts change |

## Refresh checklist

Before publishing a public update:

1. fetch both public and private repositories;
2. confirm the exact protected-`main` truth;
3. confirm active-branch status and current stop condition;
4. inspect live issue, PR, and exact-head CI state;
5. update dates only when the content was actually reconciled;
6. compare claims across `index.html`, `README.md`, and
   `PUBLIC-CASE-STUDY.md`;
7. run local-link and remote-link checks;
8. open the site at desktop and narrow mobile widths;
9. confirm no horizontal overflow, console errors, broken routes, or missing
   font fallbacks;
10. run a privacy pass for credentials, identities, machine paths, account
    information, private URLs, and edge logic;
11. keep no-profitability and no-live-execution boundaries visible;
12. publish only after the exact public diff has been reviewed.

## Future enhancement backlog

These are optional future improvements, not current claims:

- a public-safe “decision log” timeline with selected architecture decisions;
- a single sanitized evidence packet example showing expected vs actual;
- an interview-mode print/PDF export;
- a shared portfolio design token file so related public case studies feel like
  one authored system without becoming visually identical;
- automated drift checks comparing public status language with a reviewed public
  status manifest;
- an accessible social-preview image, only if explicitly commissioned.

Do not add dashboards, fake analytics, customer logos, or fabricated runtime
screenshots for visual interest. The evidence model and architecture are the
visual subject.
