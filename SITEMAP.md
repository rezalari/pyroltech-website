# Pyroltech Website, Sitemap v3 (lean)

Concise, no-redundancy IA. Cut from ~140 to ~50 focused pages while keeping full SEO/GEO coverage. Principle: **one page per real buyer intent, no duplicate axes, group the long tail into sections.** `BUILT` = live.

## What was merged or dropped (and why)
- **Feedstocks axis merged into Producers.** A waste industry *is* a feedstock source, two axes for the same intent was redundant. Feedstock keywords now live on the producer pages.
- **Locations axis dropped** (deferred). Thin, low-intent at launch; revisit for local SEO later.
- **Glossary collapsed to ONE page** with anchored terms, not a page per term.
- **Minor/emerging products folded** into the Biocarbon pillar or grouped pages (hard-carbon, supercapacitor, torrefied, asphalt, wood-tar, FT, bio-chemicals become sections, not URLs).
- **Fuels and gases grouped** (renewable fuels; clean gases) instead of one page each; SAF and hydrogen kept separate for their search volume.
- **Trust pages consolidated:** quote folds into Contact; terms + cookies into one Legal page; /process folds into Technology + How it works.
- **Industry long tail tiered:** ~14 flagship industry pages cover related sub-sectors as sections; the rest are phase-later, not separate URLs.

## Conventions (every page)
Warm light brand (`brand.html`): Archivo Expanded headlines, Inter body, IBM Plex Mono labels; deep forest `#0E4D33`, brass `#B8862F`. On-page: one H1, front-loaded answer (first 40-120 words), question H2s, FAQ + `FAQPage` JSON-LD, breadcrumbs, 3-5 internal links, one forest-green CTA. Sitewide `Organization` + `WebSite` + `BreadcrumbList`.

---

## The map (~50 pages)

### Core (10)
`/` Home `BUILT` (scroll story, globe, live Afyon counter, 3-door select) · `/technology` hub · `/global` · `/about` · `/insights` (blog) · `/contact` (incl. quote) · `/faq` · `/legal` · `/careers` · `/brand.html` `BUILT` (internal, noindex)

### Technology (4)
`/technology` hub -> `/technology/pyrolysis` · `/technology/hydrothermal` (HTC + HTL) · `/technology/gasification-upgrading` (syngas + refining). Portable vs field-size covered as sections + a `/how-it-works` explainer.

### Products (14) — hub `/products`
Pillar `/products/biocarbon` (grades as sections) with own pages for the commercial ones:
`/metallurgical-biocarbon` `BUILT` · `/activated-carbon` · `/biochar-soil-amendment` · `/recovered-carbon-black` · `/wood-vinegar` `BUILT` · `/bio-oil-biocrude` · `/renewable-fuels` (diesel/marine/naphtha) · `/sustainable-aviation-fuel` · `/green-hydrogen` · `/clean-gases` (syngas/RNG/methanol/ammonia) · `/carbon-removal-credits` · `/nutrient-recovery`

### Industries (16) — hub `/industries` (the 3 doors)
**Producers / waste creators (6 flagship):** `/industries/producers/forestry-wildfire` · `/agriculture-food` · `/tires-rubber` · `/biosolids-sludge` · `/seafood` · `/municipal-plastics` (each folds related sub-sectors as sections)
**Users / byproduct off-takers (8 flagship):** `/industries/users/steel-iron` `BUILT` · `/cement-lime` · `/refineries-fuels` · `/aviation-marine` · `/agriculture-soil` · `/power-utilities` · `/water-treatment` · `/carbon-removal-esg`
**Research (1):** `/partners/research`

### AEO surfaces (6)
`/compare` hub -> `/biocarbon-vs-met-coke` · `/biochar-vs-activated-carbon` · `/pyrolysis-vs-gasification` · `/saf-vs-renewable-diesel` · `/glossary` (single page, anchored terms)

### Proof + trust (4)
`/case-studies/afyon-turkey-2mw` (the live plant) · `/sustainability` · `/resources` (spec sheets + feedstock-to-product matrix) · `/news`

### Technical foundation
`sitemap.xml` · `robots.txt` · canonical/trailing-slash policy · human `/sitemap`.

---

## Page-type templates (keep 50 pages consistent)
- **Product:** H1 = product + what it replaces; spec card; how it's made; applications; business case; FAQ; related. Schema Product.
- **Industry (user):** H1 = the sector's outcome; problem -> our solution -> proof -> FAQ; CTA quote. Schema Service.
- **Industry (producer):** H1 = "Turn {waste} into value"; residue -> feedstock -> revenue; FAQ.
- **Compare:** H1 = the exact query; comparison table + verdict in first 100 words. Highest AEO value.
- **Hub:** short intro + card grid of spokes. CollectionPage.

## Build order
1. `BUILT`: Home, brand, metallurgical-biocarbon, wood-vinegar, steel-iron.
2. Hubs + nav routing: /products, /industries, /technology, /about, /contact.
3. Flagship money pages: cement-lime, SAF, refineries-fuels, activated-carbon, carbon-removal-credits + the Afyon case study.
4. Remaining flagship products + industries.
5. AEO (compare, glossary) + technical foundation.
6. Content engine (insights, news, freshness).
