# Pyroltech Website, Project Handoff Brief
One-file alignment doc. Feed this to any new session, collaborator or AI to continue the work exactly in line with all decisions to date. Last updated 2026-06-28.

## 1. Snapshot
- **Status:** structurally COMPLETE. All ~55 pages of the lean sitemap are built and live. Now in polish/iterate phase. Site is a private preview (`noindex,nofollow` on every page).
- **Live:** https://rezalari.github.io/pyroltech-website/
- **Repo:** https://github.com/rezalari/pyroltech-website (public repo, GitHub Pages from `main`, root)
- **Local:** `C:\Users\rezaadmin\Documents\Claude\Projects\Pyroltech\Website\`
- **Styleguide (visual source of truth):** https://rezalari.github.io/pyroltech-website/brand.html
- **Human sitemap:** /sitemap/ · IA doc: `SITEMAP.md` (v3 lean) · Design doc: `design-system/pyroltech/MASTER.md`
- **Deploy:** edit files, `git add -A && git commit && git push`; Pages rebuilds in ~30-60s. No build step, pure static HTML.

## 2. Story and strategy
- **One-liner (StoryBrand):** "The world makes waste. We make it valuable." Tagline: "CleanTech for Clean World."
- **Model:** Pyroltech is the hub between three audiences: research partners, waste producers, byproduct users. The homepage tells this as a scroll story; /industries has the three doors.
- **Founder stance (Reza):** start from zero, stay focused, execute small projects brilliantly and compound. "To fast-start: slow and focus." NEVER lead with grand size projections or hype. The site must FEEL big and expert through craft and real proof, not claims.

## 3. Brand system (mature rebrand, from a 23-competitor study)
- **Default = warm light.** Canvas `#F6F4EE`, cards `#FFFFFF`, alt surface `#ECE9E0`, ink `#16201B`, sage secondary text `#566159`, hairline `#DCD7CB`.
- **Greens:** deep forest `#0E4D33` (anchor, primary buttons, headlines accents), emerald `#1E7A52` (links/hover), mint tint `#D8E6DC`.
- **Value accent (sparing):** antique brass `#B8862F` (hover `#9C6F22`), ONLY for value moments: the word "valuable/worth", key numbers, climax CTA.
- **Forest-dark (hero band + dark toggle):** base `#0B1A13`, surface `#12281D`, text `#EDF3EE`, emerald `#3FB37C`, gold `#E0B65C`. Never near-black, never neon in UI (toned lime `#A8E063` is globe-only).
- **Type:** Archivo Expanded (H1/display), Archivo (h2/h3), Inter (body), IBM Plex Mono (eyebrows, labels, specs, live numbers). Google Fonts link is identical in every page head.
- **Logo = "Concept 2":** solid forest-green hexagon + white rising chevron + brass spark dot, inline SVG in every header + PYROLTECH wordmark in Archivo Expanded.
- **Imagery:** REAL photos only (no stocky/AI-looking, no low-res). Assets in `/assets/`: portable-road.jpg (real unit on truck), mobile-unit-forest.jpg (branded system in forest), reactor-dimple.jpg, reactor-manufacturing.jpg, plant-interior.jpg, plant-installed.jpg, unit-assembled.jpg, pyrolysis.jpg, mobile-line.jpg, logo.png.
- Radius 10-18px, soft shadows, hover translateY/scale 1.02, transitions 150-300ms, SVG icons only (never emoji), cursor: custom neon ring on homepage.

## 4. EDITORIAL HARD RULES (violations are failures)
1. **Never use an em dash.** Use commas or periods. (Reza hard rule, applies to everything, email, decks, site.)
2. **Never mention Iran** (sanctions). Heritage framing: "built across three continents: West Asia and the Middle East, from Turkey to Saudi Arabia and the UAE; Europe, from the Netherlands to Germany and Sweden; and East Asia, across Korea, Japan and China; now deployed in North America."
3. **Turkey reference plant = STEALTH:** say only "a 2 MW plant in Turkey, running non-stop." NO city (never "Afyon"), NO plant name, NO commissioning date, NO years-online figure. Invite the reader to ask (details under NDA). Live counters (kWh, CO2 avoided) are OK.
4. **Restrained, established tone.** Only these verified figures may be used: 20-30% of met coke replaceable; >30% Scope 1 CO2 cut potential; ~2.5 t CO2 removed per tonne biocarbon (IPCC-recognised, credit-eligible); met coke ~$240-290/t; credit index ~$130-165/tCO2; activated-carbon market ~$5.6B to ~$11.9B by 2034; BC treated-wood tipping ~$110-170/t before hauling; rCB ~EUR3.2B addressable at ~20% substitution; 2 MW live plant; 20+ years; three continents. Everything else stays qualitative. Do NOT use the debunked "$290/t disposal" figure.
5. `hello@pyroltech.com` is a PLACEHOLDER contact address, confirm the real one before go-live.

## 5. Site structure (v3 lean, ALL BUILT)
- **Core:** / (scroll story + cobe globe + live Turkey counter + 3 doors) · /products/ · /industries/ (#producers #users #research) · /technology/ · /about/ · /contact/ · /global/ · /how-it-works/ · /faq/ · /insights/ · /news/ · /resources/ · /sustainability/ · /careers/ · /legal/ · /sitemap/ · /partners/research/ · brand.html
- **Products:** biocarbon (pillar), metallurgical-biocarbon (flagship), activated-carbon, biochar-soil-amendment, recovered-carbon-black, wood-vinegar, bio-oil-biocrude, renewable-fuels, sustainable-aviation-fuel, green-hydrogen, clean-gases, carbon-removal-credits, nutrient-recovery
- **Industries/producers:** forestry-wildfire, agriculture-food, tires-rubber, biosolids-sludge, seafood, municipal-plastics
- **Industries/users:** steel-iron (flagship), cement-lime, refineries-fuels, aviation-marine, agriculture-soil, power-utilities, water-treatment, carbon-removal-esg
- **Technology:** pyrolysis, hydrothermal (HTC+HTL), gasification-upgrading
- **AEO:** /compare/ + biocarbon-vs-met-coke, biochar-vs-activated-carbon, pyrolysis-vs-gasification, saf-vs-renewable-diesel · /glossary/ (single page, anchored terms)
- **Proof:** /case-studies/turkey-2mw/ (stealth)
- **Foundation:** robots.txt, sitemap.xml (canonical https://pyroltech.com URLs)

## 6. New-page recipe (keeps everything consistent)
1. Copy a pattern: product page = `products/carbon-removal-credits/index.html`; industry page = `industries/users/steel-iron/index.html`. All content pages share `assets/page.css`.
2. Depth rule: page at /x/ uses `../` prefix for all internal links and css; /x/y/ uses `../../`; /x/y/z/ uses `../../../`.
3. Every page: noindex meta (until launch), <title> <60 chars ending "| Pyroltech", meta description, canonical https://pyroltech.com{path}, the standard font link, standard header/nav/footer, breadcrumb.
4. SEO/GEO pattern: ONE h1; front-loaded direct answer in the first 40-120 words; question-style h2s; spec-card aside where useful; statistics with restraint; FAQ block + matching FAQPage JSON-LD; Organization + BreadcrumbList JSON-LD; 3 Related links; one forest-green CTA to /contact/.

## 7. Homepage specifics
- Hero = forest-dark band with **cobe** WebGL dotted globe (drag-to-spin, 10 markers: Turkey, Riyadh, Dubai, Netherlands, Berlin, Stockholm, Seoul, Tokyo, Beijing, Vancouver). GSAP ScrollTrigger reveals + count-ups, native scroll (Lenis was removed for smoothness), scroll progress bar, custom cursor, dark/light toggle (light default).
- Live plant section: pulsing LIVE badge, "A 2 MW plant in Turkey, running non-stop", live kWh + CO2 counters (JS computes from 2 MW × elapsed time; internal start date Mar 2021 and CO2 factor 0.44 kg/kWh are UNCONFIRMED, verify with Fred; years deliberately not shown).
- Logo wall = 12 grayscale placeholders awaiting Fred's list (name, region, role, logo file per company; universities UBC/UNB row exists).

## 8. Open items
1. Fred's partner/client logos for the proof wall (and by-region reveal on the globe, original concept).
2. Confirm live-counter assumptions (start date, 2 MW continuous, CO2 factor) with Fred.
3. Real contact email + any phone/address for /contact/ and Organization schema.
4. Copy-polish pass page by page; add more real photos to inner pages; possible hero video loop (Fred's videos not yet downloaded).
5. Go-live checklist: remove noindex sitewide, point pyroltech.com DNS at Pages (or move host), submit sitemap.xml to Google Search Console, then monthly freshness refreshes on top pages.
6. Pitch decks in `...\Pyroltech\PitchDecks\` still use the OLD teal brand, re-skin to this system when needed.

## 9. Context worth knowing
- The ui-ux-pro-max skill is installed in this project (`.claude/skills/`, gitignored). Design-system engine: `python .claude/skills/ui-ux-pro-max/scripts/search.py "<query>" --design-system`.
- SEO/GEO/AEO strategy (verified research): separate page per intent, pillar-and-cluster, FAQPage schema everywhere (highest AI-citation rate), front-loaded answers, statistics + cited sources, freshness; llms.txt intentionally skipped.
- Repo was private, flipped public ONLY because free-plan GitHub Pages requires it; noindex keeps it out of search. To re-privatize: `gh repo edit rezalari/pyroltech-website --visibility private` (kills the live URL unless on GitHub Pro).
