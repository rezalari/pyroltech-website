# Pyroltech Website, Sitemap v2

Pillar-and-cluster information architecture, upgraded 2026-06-27 from competitor research + the mature rebrand. ~140 pages. Most spokes are template + data, not hand-built.

`NEW` = added in v2. `BUILT` = live now. Everything follows the brand in `brand.html` and the on-page pattern below.

---

## Conventions (apply to every page)

- **Brand:** warm light default `#F6F4EE`, deep forest green `#0E4D33` anchor, antique brass `#B8862F` value accent, Fraunces headlines + Inter body + IBM Plex Mono labels. See `brand.html`.
- **URL:** lowercase, hyphenated, hub/spoke (e.g. `/products/metallurgical-biocarbon`). Clean folder URLs.
- **On-page pattern (SEO + GEO + AEO + human):**
  1. One `<h1>`, descriptive `<title>` (<60 chars), meta description, canonical.
  2. **Front-loaded answer** in the first 40-120 words (this is what AI engines quote).
  3. **Question-style H2/H3s** (the buyer's real prompt).
  4. Scannable body: short intro -> spec card / cards / key numbers -> real photo.
  5. **FAQ block + `FAQPage` JSON-LD** on every high-value page.
  6. Sitewide schema `Organization` + `WebSite` + `BreadcrumbList`; per page `Product`/`Service`/`Article`/`HowTo`.
  7. Add **statistics + cited sources**; keep fresh (refresh top pages monthly).
  8. **3-5 internal links** wiring feedstock -> tech -> product -> industry; every spoke links back to its hub. No orphans.
  9. Breadcrumbs, one primary CTA (forest green), accessibility (contrast, focus, alt text).

---

## The map

### Home & Core
- `/` Home `BUILT` (scroll story + globe + live Afyon counter)
- `/solutions` the 3-door self-select
- `/technology` hub -> `/pyrolysis` `/hydrothermal-carbonization` `/hydrothermal-liquefaction` `/gasification` `/downstream-upgrading` `/portable-pyrolysis-unit` `/field-size-plants` `/remote-operations` `/licensing-epc`
- `/partners` `NEW` hub -> `/partners/research` (`/grants` `/pilots` `/publications`), `/partners/channel` `NEW`
- `/global` interactive globe + live plant data + 20-yr timeline
- `/case-studies` hub -> `/case-studies/afyon-turkey-2mw` `NEW` (the live plant, our strongest proof)
- `/about` (+ `/about/team`)
- `/insights` blog hub (topic clusters, case studies as cornerstone)
- `/news` `NEW` hub -> `/news/{slug}` `NEW` (press, funding, milestones; distinct from educational insights)
- `/investors` `NEW`
- `/sustainability` `NEW` hub -> `/sustainability/lifecycle-assessment` `NEW`, `/sustainability/certifications` `NEW`
- `/contact` (+ `/contact/thank-you` `NEW`), `/quote` `NEW`, `/how-it-works` `NEW`, `/process` `NEW`, `/pricing` `NEW` (cost-drivers guide)
- `/careers`, `/faq`, `/privacy`, `/terms`, `/cookies`, `/search`, `/accessibility` `NEW`, `/404`
- `/brand.html` `BUILT` internal styleguide (noindex), `/sitemap` `NEW` (human HTML)

### Products (hub `/products`)
Biocarbon pillar `/products/biocarbon` -> `/metallurgical-biocarbon` `BUILT` · `/biochar-soil-amendment` · `/activated-carbon` · `/biochar-construction` · `/biochar-water-soil-remediation` · `/biochar-animal-feed` · `/hard-carbon-sodium-ion` · `/supercapacitor-carbon`
Other products: `/recovered-carbon-black` · `/hydrochar` · `/bio-oil` · `/htl-biocrude` · `/renewable-diesel` · `/sustainable-aviation-fuel` · `/renewable-marine-fuel` · `/renewable-naphtha` · `/wood-vinegar` `BUILT` · `/bio-based-chemicals` · `/wood-tar-bio-pitch` · `/syngas` · `/green-hydrogen` · `/renewable-natural-gas` · `/green-methanol` · `/green-ammonia` · `/fischer-tropsch-fuels` · `/heat-and-power` · `/carbon-removal-credits` · `/nutrient-recovery` · `/torrefied-biomass` `NEW` · `/biochar-asphalt-bitumen` `NEW`

### Industries / Producers (waste creators) `/industries/producers/{slug}`
forestry-wood-products · wildfire-land-fuel-management · agriculture-field-crops · agri-food-processing · breweries-distilleries · sugar-ethanol · livestock-poultry · seafood-fisheries · pulp-paper · municipal-solid-waste · biosolids-wastewater-sludge · end-of-life-tires-rubber · plastics-packaging · oil-gas-petroleum · coal · mining-metallurgy-residues · biogas-digestate · construction-demolition · textiles · palm-vegetable-oil · cannabis-greenhouse-horticulture · medical-hospital-waste · landfill-operators · ports-airports-logistics · remote-indigenous-communities-islands · rail-wood-ties · composting-organics-processors

### Industries / Users (byproduct off-takers) `/industries/users/{slug}`
steel-iron `BUILT` · cement-lime · tire-rubber-rcb · aviation-saf · shipping-marine · refineries-fuels · chemicals-petrochemicals · hydrogen-heavy-transport · power-utilities · agriculture-soil-fertilizer · water-wastewater · construction-materials · carbon-removal-esg · environmental-remediation · activated-carbon-market · greenhouse-horticulture · animal-feed-bedding · plastics-circular · asphalt-roofing · battery-electrode-materials · mining · forestry-pellet-bioenergy

### NEW discovery axis: Feedstocks `/feedstocks/{material}`
Buyers and AI search by material, not just industry. e.g. `forestry-residue` · `rice-husk` · `sewage-sludge` · `scrap-tires` · `manure` · `nut-shells` · `bagasse` · `mixed-plastics` · `food-waste` · `algae`

### NEW discovery axis: Locations `/locations/{region}`
e.g. `canada` · `british-columbia` · `alberta` · `saskatchewan` · `turkey` (local SEO + the global footprint story)

### NEW AEO surfaces
- Compare `/compare/{x-vs-y}`: `biocarbon-vs-metallurgical-coke` · `biochar-vs-activated-carbon` · `pyrolysis-vs-gasification` · `biochar-vs-compost` · `saf-vs-renewable-diesel`
- Glossary `/glossary` -> `/glossary/{term}`: pyrolysis · biochar · met-coke · carbon-removal · HTC · HTL · syngas · wood-vinegar · CORC ...
- Resources `/resources` -> `/resources/spec-sheets/{product}` `NEW` (downloadable datasheets) · `/resources/feedstock-compatibility` `NEW` (the feedstock -> tech -> product matrix tool) · `/resources/white-papers` `NEW`

### Technical foundation `NEW`
`sitemap.xml` · `robots.txt` (declare sitemap, block `/search`) · canonical + trailing-slash policy · `WebSite` + `SearchAction` schema.

---

## Overlap reconciliations (fix cannibalization)
Three topics exist as both a PRODUCT and an INDUSTRY page. Keep both, split by intent, self-canonical, cross-link:
- `/products/activated-carbon` (what it is, specs, buy) vs `/industries/users/activated-carbon-market` (your sector's problem -> our solution).
- `/products/carbon-removal-credits` (the credit product) vs `/industries/users/carbon-removal-esg` (ESG buyers' need).
- `/products/biochar-construction` (the material) vs `/industries/users/construction-materials` (the sector) vs `/industries/producers/construction-demolition` (the waste source). Distinct intents, link the trio.

---

## Page-type templates (so 140 pages stay consistent)

**Product page** (e.g. metallurgical-biocarbon): title `"{Product} | {benefit} | Pyroltech"`; H1 = product + what it replaces; front-load "what it is + who buys it"; spec card; how it's made (4 steps); applications grid; business case; FAQ; related (hub, buyer industry, tech, feedstock, compare); schema Product + BreadcrumbList + FAQPage.

**Industry / User page** (e.g. steel-iron): title `"{Product} for {industry} | Pyroltech"`; H1 = the sector's outcome; front-load the sector pain -> our solution; "the problem", "our solution", proof, FAQ; CTA quote; schema Service + BreadcrumbList + FAQPage.

**Industry / Producer page**: H1 = "Turn {waste} into value"; front-load the residue -> feedstock -> revenue flip; what we take, what it becomes, the economics, FAQ.

**Feedstock page**: H1 = "{Material} to {best products}"; the material -> best tech -> outputs -> off-takers; links to those product + industry pages.

**Compare page**: H1 = the exact query ("Biocarbon vs metallurgical coke"); a comparison table + a clear verdict in the first 100 words; FAQ. Highest AEO value.

**Glossary term**: H1 = the term; a 1-2 sentence definition first (snippet-ready); then detail + links to the relevant product/tech pages.

**Hub / Collection**: short intro + a card grid of its spokes; CollectionPage schema; routes humans + passes link authority.

---

## Build phases
- **P0 Foundation:** robots.txt, sitemap.xml, HTML /sitemap, canonical policy, page-type templates. (product + industry templates now built)
- **P1 Launch core:** `/` `BUILT`, hubs (/products, /industries, /technology, /solutions), /about, /contact, /quote, /how-it-works, trust pages.
- **P2 Flagship products + tech:** metallurgical-biocarbon `BUILT`, wood-vinegar `BUILT`, SAF, the 5 technology pages.
- **P3 Flagship industries (both sides):** steel-iron `BUILT`, cement-lime, forestry, wildfire, tires, seafood; the Afyon case study.
- **P4 Long-tail waves:** remaining ~25 producer + ~20 user spokes (programmatic from the matrix).
- **P5 New axes + AEO:** /feedstocks, /locations, /compare, /glossary, /resources.
- **P6 Content engine:** /insights, /news, freshness, link-building.
