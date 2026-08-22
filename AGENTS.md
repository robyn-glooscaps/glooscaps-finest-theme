# AGENTS.md

## Authority and scope

Read `README.md` and every issue specification before changing files.

This repository is a review and recovery workspace for the Glooscap's Finest Shopify informational storefront. Shopify itself is outside the Cloud task's write scope unless a later issue explicitly provides a safe unpublished theme target and separately authorizes that mutation.

## Hard constraints

- Never edit, publish, duplicate, delete, or otherwise mutate the live MAIN Shopify theme.
- Never activate products, change product status, alter pricing/inventory, enable checkout, or change store access.
- Never place credentials, tokens, environment files, customer data, Shopify exports containing secrets, or unrelated filesystem content in this repository or recovery artifacts.
- Never redesign, redraw, recolour, crop, trace, vectorize, AI-regenerate, or overwrite supplied logo files.
- Never invent Mi'kmaw language, teachings, Medicine Wheel meanings, ceremonial content, founder biography, maker affiliations, health claims, regulated claims, product facts, addresses, hours, contact details, prices, strengths, ingredients, directions, or warnings.
- Never call review-pending work approved, compliant, production-ready, deployed, or launched.
- Never merge or modify `main`.

## Brand system

- Formal public brand name: `Glooscap's Finest`.
- Technical handles and filenames may retain `glooscaps` for compatibility.
- Preserve `EST. 1752` exactly as part of the official emblem. It is a Treaty heritage reference, not the founding year of the present business.
- Preserve official logo artwork exactly.
- Use the modern heritage apothecary system:
  - Medicine Wheel Yellow `#FDF116`
  - White `#FFFFFF`
  - Red `#F60405`
  - Black `#070707`
  - Warm Cream `#F5F0E7`
  - Parchment `#E7D9C8`
  - Charcoal `#1B1A18`
  - Cedar `#465447`
  - Stone `#9A9287`
- Display/editorial: Noto Serif Bold, Georgia fallback.
- Body/interface: Noto Sans, Arial fallback.
- Use restrained four-colour rail, fine rules, negative space, archival paper tones, tactile materials, and evidence-backed botanical engraving.
- Avoid generic dispensary visuals, smoke effects, neon, gradients, cannabis-leaf wallpaper, faux-vintage distress, unapproved cultural motifs, and excessive ornament.

## Content and adult boundary

- General store, art, maker, non-cannabis, and educational content should remain independently navigable.
- Direct adult-use product content requires an explicit 19+ classification path.
- The current live theme uses heuristic title/type/tag/collection matching because `custom.restriction_classification` definitions do not yet exist. Treat this as a launch blocker.
- Adult-use product pages are informational only and must not expose checkout, prices, quick-add, quantity, pickup, recommendations, search leakage, or cart pathways.
- Educational content must remain factual, sourced, limitation-aware, and separated from finished-product promises.
- Cultural biography and community copy require traceable sources and final human approval.

## Workflow

- Work on a separate `codex/*` branch.
- Preserve existing source files and hashes unless the issue explicitly authorizes an edit.
- Prefer deterministic scripts, manifests, and validation over manual-only changes.
- Add tests for classification, restricted-surface leakage, navigation, accessibility, and responsive behavior when applicable.
- Put review-only outputs under `project-artifacts/<task-name>/`.
- If PR creation or pushing fails, still create:
  - a downloadable ZIP of changed files and generated review artifacts;
  - a binary-capable patch;
  - a checksum manifest;
  - a concise validation report.
- Inspect tracked, untracked, and explicitly allowed ignored artifact paths before claiming outputs are missing.

## Required final report

Report exact changed files, untouched/protected files, tests run, unresolved blockers, artifact paths, recovery links, and confirmation that Shopify, live theme state, products, collections, pages, store access, and `main` were not changed.
