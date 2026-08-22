# Glooscap's Finest Shopify Theme

This repository is the safe handoff workspace for the Glooscap's Finest informational Shopify storefront.

## Live store state captured 2026-08-22

- Store: `glooscapsfinest.com`
- Shopify shop: `glooscaps-finest420.myshopify.com`
- Public storefront is password protected.
- Current MAIN theme: `Glooscaps Informational Build` — `gid://shopify/OnlineStoreTheme/186587480384`
- Current MAIN theme inventory: 436 files.
- Catalogue: 114 products — 67 draft, 47 archived, 0 active.
- Collections: 25 total; all are published in Shopify admin, but product availability remains closed because no products are ACTIVE.
- Pages: 37 total — 23 published, 14 unpublished.
- Custom data gap: no product restriction-classification metafield definition, no collection/page custom definitions, and no metaobject definitions.
- The current selective 19+ logic therefore falls back to title/type/tag/collection heuristics.

## Purpose of this repository

Preserve the Glooscap's Finest-specific theme layer and brand assets so Codex Cloud work can be reviewed, recovered, and applied without editing the live Shopify theme.

This repository is not a deployment source yet. It begins with a controlled snapshot of custom Glooscap's Finest code and supplied brand assets. The full commercial theme dependency is intentionally not copied here.

## Non-negotiable safety boundary

- Do not publish or edit the MAIN Shopify theme.
- Do not activate products, enable checkout, alter inventory, or change commerce settings.
- Do not describe draft/review work as launched, approved, compliant, or production-ready.
- Work on a separate branch and do not merge to `main`.
- Preserve downloadable recovery artifacts even when PR creation is unavailable.

## Brand direction

Use the current internal foundation: a modern Mi'kmaw-owned trading post and modern heritage apothecary—premium, warm, useful, culturally rooted, and factual.

- Formal written brand: **Glooscap's Finest**
- Official emblem text: **GLOOSCAP'S FINEST / EST. 1752**
- Brand line: **Rooted in knowledge. Made with care.**
- Palette: Medicine Wheel yellow, white, red, and black, supported by warm cream, parchment, charcoal, cedar, and stone.
- Typography: Noto Serif for display/editorial roles; Noto Sans for body/interface roles; Georgia/Arial fallbacks.
- Avoid generic dispensary green, neon, smoke effects, cannabis-leaf wallpaper, pan-Indigenous motifs, invented teachings, and unsupported health claims.

## Current priority

1. Preserve and audit the custom theme source.
2. Replace heuristic adult-content classification with an explicit custom-data plan.
3. Finish the homepage, brand asset implementation, and Community & Makers architecture.
4. Run mobile/accessibility/navigation/commerce-leak regression QA.
5. Produce a launch-readiness packet; do not publish.
