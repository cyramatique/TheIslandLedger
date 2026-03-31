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
