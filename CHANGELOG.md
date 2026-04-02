# Changelog

All notable changes to The Island Ledger & The Resident Representatives are documented here.  
Format: `[Date] — Description · Source`

---

## 2026-03-31 — Initial public release

### New: Unified single-file format
- Combined The Island Ledger (network diagram) and The Resident Representatives (timeline) into a single self-contained HTML file: `epstein-unified.html`
- Fixed-top navigation bar switches between the two pages without reload
- D3 simulation receives an alpha kick on return to network page to restore animation

### New: The Resident Representatives — timeline rebranded
- Previously: `epstein-timeline-v5.html` (standalone dark-theme file)
- Now integrated with Mar-a-Lago palette matching the network diagram
- Title updated to *The Resident Representatives & Affiliates*
- Header copy restructured: Public Record · Mar 2026 / The Three Tracks as bullet list
- Full contrast pass on Document Record: evidence cards, quote blocks, verdict strips, reference text — all remapped from dark-on-black to readable mahogany-on-parchment

### Network diagram — 122 individuals (clean, deduplicated)
Previous "122" count was inflated by 7 duplicate/placeholder nodes. After cleanup and addition of 9 new individuals, true count is 122.

**Duplicates removed:** botstein/bothstein, blaine/davidblaine, band/dougband, chopra/chopra2, wassmerman/wasserman, chollet (phantom Ruemmler duplicate), brunel2 (r:0 placeholder)

**9 new individuals added:**
- Andrew Farkas (co-owned St Thomas marina with Epstein, stayed on island)
- Soon-Yi Previn (corresponded with Epstein, thanked him for Bard College admission)
- Tsakhiagiin Elbegdorj (President of Mongolia, attended Manhattan dinner with Epstein and Barak)
- Steve Tisch (New York Giants co-owner, named 400+ times, NFL investigating)
- Lawrence Delson (FIT professor, suspended following file revelations)
- John de Jongh Jr. (USVI Governor, Epstein paid university tuition for his children)
- David Hanson (Hanson Robotics, co-solicited Epstein funding with Goertzel for Sophia robot)
- Brett Ratner (film director, named in files)
- Kevin Warsh (Fed Reserve chair nominee, Epstein St Barth's guest list 2010)

**4 existing nodes updated with richer detail:**
- Tom Pritzker → `stripped` (resigned Hyatt Hotels executive chairman Feb 2026; helped arrange SE Asia trip to find Epstein a girlfriend)
- Brad Karp → full email detail added ("once in a lifetime evening"; visa revocation request; son's job request on Allen film)
- Dean Kamen → `stripped` (resigned Beta Technologies board Feb 2026; resigned FIRST board Mar 11 2026)
- Robert Trivers → explicit 2015 Reuters quotes defending Epstein's crimes added

### New: Incarcerated status category
- Black `#111111` nodes for Maxwell, Cosby, Weinstein
- Separate filter chip in toolbar
- Distinct consequence block styling

### New: Travel record tags in every dossier
- ✈ Plane and ⛵ Island status for 108 of 122 individuals
- Colour-coded: crimson = confirmed, navy = denied, gold = unclear

### New: DOJ Pinpoint deep links
- Every dossier has a "Search in DOJ Epstein files ↗" button
- Links directly to `journaliststudio.google.com/pinpoint` with the person's name pre-searched
- Hidden for Epstein centre node

### Design
- Mar-a-Lago palette throughout: parchment `#F5F0E8`, hunter green `#1B3A2D`, aged gold `#B8963E`
- Playfair Display (display) + Cormorant Garamond (body) + Cormorant SC (labels)
- Linen texture overlay, gold corner flourishes, double-rule border frame
- Node outlines removed — fill colour carries status coding
- Epstein centre node: gold `#C9A84C`
- Signature: *Designed by Cyramatique* · `rgba(0,97,161,1)` brand blue · bottom left
- Zone labels: 13.2px, 70% opacity, "Social / Cultural" properly labelled
- Dossier panel: ✦ bullet lists for connection and consequence sections

### CSV
- `epstein-accusations.csv` regenerated cleanly from HTML source
- 122 rows, 10 columns: name, title, sector, status, plane, island, connection_summary, consequence, badges, source
- Clean 1:1 match with diagram — no legacy rows from removed duplicates

---

## Status changes tracked in this release

| Person | Previous | New | Date | Reason |
|--------|----------|-----|------|--------|
| Børge Brende | Active | Removed | Feb 2026 | Resigned WEF CEO |
| Larry Summers | Active | Removed | Feb 2026 | Resigned all Harvard roles, stepped down from OpenAI |
| Tom Pritzker | Active | Stripped | Feb 2026 | Resigned Hyatt executive chairman |
| Dean Kamen | Active | Stripped | Feb–Mar 2026 | Resigned Beta Technologies board + FIRST board |
| Deepak Chopra | Active | Stripped | Mar 2026 | UCSD ended affiliation |
| Steve Tisch | — | Stripped | Feb 2026 | NFL opened investigation |
| Lawrence Delson | — | Stripped | Feb 2026 | FIT suspended, investigation launched |
| Kathryn Ruemmler | Active | Removed | Feb 2026 | Resigned Goldman Sachs GC |
| Casey Wasserman | Active | Stripped | Feb 2026 | Sold Wasserman Management stake |
| Ghislaine Maxwell | Removed | Incarcerated | — | Serving 20-year federal sentence |
| Harvey Weinstein | Removed | Incarcerated | — | Serving 16-year state sentence |
| Bill Cosby | Removed | Incarcerated | — | Serving state sentence |

---

## Outstanding — to be updated when resolved

- GAO investigation into DOJ's EFTA compliance (opened Mar 11 2026, ongoing)
- Bondi subpoena — outstanding, not complied with as of Mar 2026
- Missing FBI 302s from South Carolina accuser — withheld by DOJ, NPR investigation ongoing
- Thorbjørn Jagland trial outcome (charged with aggravated corruption Feb 2026)
- Terje Rød-Larsen and Mona Juul criminal proceedings (Norway, ongoing)
- Andrew Mountbatten-Windsor — released without charge, remains under investigation

---

*Corrections and additions: open an issue on this repository*

---

## 2026-04-01 — v1.1 · Mobile, sidebar, and UX improvements

## 2026-04-02 — Breaking: Bondi fired

### Timeline — new entry added
- **Apr 2 2026 · AG fired** — Pam Bondi removed as Attorney General after 14 months.
  Epstein files handling cited as the primary cause: her Feb 2025 "client list on my 
  desk" claim, the subsequent DOJ reversal, the EFTA it triggered, and the House 
  Oversight subpoena she had not complied with. Last day technically Apr 1. Only an 
  estimated 2% of total Epstein data released under her tenure. Todd Blanche (Trump's 
  former personal attorney) named acting AG. Lee Zeldin (EPA) frontrunner for 
  permanent replacement. Rep. Khanna called it the direct result of a "cover-up." 
  Rep. Garcia warned the firing does not get her out of testifying under oath.
- Sources: CNN, NBC News, NPR, CBS News, CNBC, Euronews, Newsweek · Apr 2 2026

### Sidebar updated
- Bondi subpoena chip: "Outstanding — not complied" → "Bondi fired Apr 2 2026 · subpoena unresolved"

### Note on placement
- Timeline only — Bondi is not named in the Epstein files and has no documented 
  personal connection to Epstein. Her relevance is as the AG who oversaw the EFTA 
  release process and was fired for mishandling it.

### File renamed
- `epstein-unified.html` → `index.html` for GitHub Pages compatibility
- Live at `https://[username].github.io/epstein-files/`

### New: Mobile responsive layout (≤768px)
- **The Island Ledger** — D3 diagram replaced on mobile with a searchable list of all 121 individuals
  - Tap any name to expand inline dossier: title, travel tags, connection summary, consequence, DOJ Pinpoint link
  - Search box filters list live as you type
  - Status dot colour preserved from desktop diagram
- **The Resident Representatives** — full mobile pass
  - Sidebar hidden on mobile (proceedings status + EFTA chips desktop-only)
  - Timeline collapses to single column, tightened padding
  - Evidence grid goes single column
  - Tab bar horizontally scrollable

### New: Timeline right sidebar
- **⚖ Proceedings status** — 10 live status items: Trump v. Dow Jones, Wolff v. Melania, Bondi subpoena, GAO investigation, Missing FBI 302s, Grand jury unsealing, MCC guards indictment, Jagland charges, Rød-Larsen/Juul investigation, Andrew/Mandelson arrests
- **📄 Key EFTA documents** — 8 document reference chips with one-line descriptions, colour-coded by severity (red / gold / green)
- Sidebar is sticky — stays in view while scrolling through timeline entries

### New: Clickable names in timeline
- 48 name links across timeline `.cb` entries wired to inline mini-dossier
- Clicking a name (Trump, Maxwell, Wolff, Giuffre, Acosta, Lutnick etc.) updates the right sidebar with that person's full dossier — title, travel tags, connection summary, consequence, Pinpoint link — without leaving the timeline page
- ✕ close button returns sidebar to default proceedings/documents view

### UX fixes
- Scroll restored on The Resident Representatives page (network CSS `overflow:hidden` was leaking globally)
- Dossier panel CSS restored after being dropped in a previous update (`.dos-bullets`, `.dos-travel`, `.dos-travel-tag`)
- Orphaned legend HTML fragment removed — was rendering as visible text in top-right corner and disrupting flex layout
- Timeline right column empty gutter replaced with functional sidebar
- Nested `tl-name-link` spans cleaned (multiple regex passes had triple-wrapped some names)
- `getElementById` null guards added throughout — prevents crash when timeline page is not yet visible

### Typography
- All font sizes increased ~15% across both pages for readability
- Affects: nav bar, dossier panel, travel tags, sidebar chips, legal track dividers, timeline card text, evidence cards, claim quotes

### Node count
- Display count corrected: toolbar now shows `121 individuals + Epstein` (Epstein excluded from count as centre node)
- Underlying data unchanged at 122 total nodes

