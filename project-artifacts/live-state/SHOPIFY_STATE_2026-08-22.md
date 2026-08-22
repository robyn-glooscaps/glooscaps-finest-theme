# Live Shopify state — 2026-08-22

Read-only snapshot captured from the connected Shopify Admin API. This file is evidence for Cloud tasks; it is not permission to mutate Shopify.

## Store

| Field | Value |
|---|---|
| Name | Glooscap's Finest |
| Primary domain | glooscapsfinest.com |
| Plan | Basic |
| Currency | CAD |
| Timezone | ADT |
| Country | Canada |
| Public access | Password protected |

## Themes

| Theme | Shopify theme ID | Role | Last updated |
|---|---|---|---|
| Glooscaps Informational Build | 186587480384 | MAIN | 2026-08-15 |
| Copy of Glooscaps Informational Build | 186989478208 | UNPUBLISHED | 2026-07-26 |
| Glooscaps Finest — Phase 7 Preview — 2026-08-05 | 187362574656 | UNPUBLISHED | 2026-08-05 |
| Glooscaps Finest — Phase 7 Preview — 2026-08-05 | 187363164480 | UNPUBLISHED | 2026-08-06 |
| Flora | 185416581440 | UNPUBLISHED | 2026-07-27 |

The MAIN theme contains 436 files:

- assets: 113
- blocks: 93
- config: 2
- layout: 2
- locales: 51
- sections: 51
- snippets: 105
- templates: 19

Most Glooscap's Finest-specific source was last updated 2026-07-19. The password template was updated 2026-08-15.

## Catalogue

| Status | Count |
|---|---:|
| Total products | 114 |
| ACTIVE | 0 |
| DRAFT | 67 |
| ARCHIVED | 47 |
| Tagged Catalog | 97 |
| Ready for Review | 62 |
| Needs Photos | 93 |
| Needs Pricing | 6 |
| Needs Product Details | 5 |

No product should be activated by Cloud tasks.

## Collections

25 collections exist and all 25 are published in Shopify admin. Relevant populated collections include:

| Collection | Products |
|---|---:|
| Catalog | 97 |
| Internal — CBD | 37 |
| Internal — 1:1 THC/CBD | 37 |
| Pain & Relief | 27 |
| Edibles | 25 |
| Bath & Body | 13 |
| Extracts & Concentrates | 9 |
| Capsules | 8 |
| Oils & Tinctures | 8 |
| Flower | 3 |
| Pet Products | 2 |
| Vapes | 2 |
| Needs Photos | 93 |
| Needs Pricing | 6 |

Seven legacy collections are empty and prefixed `Legacy —`. `Healthcare example products` and `Herbal Remedies` are empty. `Home page` contains one product.

The current admin Main menu contains a `Shop` parent pointing to `/collections/catalog` with collection children. The custom Glooscap's header is hardcoded to homepage anchors and About/Contact instead of this admin menu. Navigation authority therefore needs reconciliation before launch.

## Pages

- 37 total
- 23 published
- 14 unpublished

Published information architecture includes:

- The Glooscaps Library
- Hemp 101
- CBD Guide
- THC Guide
- Full Spectrum vs Broad Spectrum vs Isolate
- Botanical Ingredients
- Frequently Asked Questions
- RSO
- Topical Wellness
- Pain Cream
- Pain Spray
- Roll-On Pain Relief
- Hemp Oils & Tinctures
- Capsules
- Bath & Body Collection
- Suppositories
- Edibles
- Bear Grease
- Colloidal Silver
- Find Your Format
- Botanical Collection
- About Us
- Contact

Legacy guides and old utility pages remain unpublished.

## Custom-data architecture

### Product custom metafield definitions

The store has 15 legacy/theme custom definitions for reviews, collapsible rows, emoji benefits, and variation statistics.

It does **not** have `custom.restriction_classification` or another explicit product adult-content classification definition.

### Collection and page definitions

No custom metafield definitions exist for collections or pages.

### Metaobjects

No metaobject definitions exist. The planned artist/maker/community system has not been built in Shopify admin.

## Current restriction implementation

The live theme includes:

- `snippets/glooscaps-age-gate.liquid`
- `snippets/glooscaps-product-restricted.liquid`
- restricted product, collection, and reference-guide handling
- search, collection-list, cart, and 404 message templates
- hidden price/buy/quantity/pickup/swatches/SKU/rating UI for restricted products

Because explicit classification data is absent, classification falls back to title, product type, tags, and collection handles. This heuristic boundary remains a launch blocker until deterministic custom data and regression tests exist.

## Current custom theme layer

The controlled snapshot in this repository preserves the current Glooscap's-specific sections, snippets, JSON templates, and header/footer wiring. It does not include the full third-party/commercial base theme.

Cloud tasks must treat the snapshot as review source, not a complete deployable theme.
