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


---

## 2026-04-02 — Breaking: Bondi fired

### Timeline — new entry added
- **Apr 2 2026 · AG fired** — Pam Bondi removed as Attorney General. Multiple sources confirm Epstein files handling was central to her firing. Her Feb 2025 "client list on my desk" statement, the subsequent DOJ reversal, and her failure to comply with the House Oversight subpoena all cited. Todd Blanche named acting AG. Lee Zeldin (EPA) frontrunner to replace permanently.
- Sources: CNN, NBC News, NPR, CBS News, CNBC · Apr 2 2026

### Sidebar updated
- Bondi subpoena status: "Outstanding — not complied" → "Bondi fired Apr 2 2026 · subpoena unresolved"

### Note on placement
- Bondi added to timeline only — she is not named in the Epstein files directly and has no documented personal connection to Epstein. Her relevance is as the AG who oversaw and mishandled the EFTA release process.

---

## 2026-04-09 — Melania White House statement

### Timeline — new entry added
- **Apr 9 2026 · Melania statement** — First Lady delivers unscheduled White House address denying Epstein ties. Acknowledges 2002 "Love Melania" email to Maxwell, calls it trivial. Calls on Congress to hold public survivor hearings — directly contradicting administration messaging. Trump said he didn't know about the statement; White House said he did. Bipartisan support from Mace and Garcia for hearing call. Survivors mixed; Gloria Allred called on Melania to testify herself.
- Sources: CNN, CNBC, Fortune, NPR, ABC News, White House transcript · Apr 9–10 2026

### Legal track updated
- Wolff v. Melania Trump entry: noting Melania's Apr 9 on-record denial and Maxwell email acknowledgment as new material in the proceedings

### Note on Ivanka / DOAC
- Ivanka Trump appeared on Diary of a CEO Apr 9 — personal/family content only, no Epstein material. Not added to the ledger.

---

## 2026-04-23 — v1.3 · Proximity tiers, About modal, Epstein Exposed, travel data audit

### Renamed: The Resident Representatives → Trump Timeline
- Nav button, page H1, browser title, and GA tracking label all updated
- Internal page ID (`page-timeline`) unchanged for stability
- All future references use Trump Timeline

### New: Proximity tier system
The diagram now encodes relationship closeness through node distance and size — nodes physically closer to Epstein had more direct documented contact.

**Three tiers based on editorial judgement:**
- **Tier 1 — Innermost (28 nodes):** Direct operational role, enabler badge, or both plane AND island confirmed. Nodes render at 1.5× base size, pulled to ~95px from centre. Includes Maxwell, Wexner, Staley, Black, Pritzker, Barak, Brunel, Kellen, Groff, Dershowitz, Acosta, Ito, Krauss, Summers, Andersson, D'Agostino, Jarecki, Seckel, Weinstein and others.
- **Tier 2 — Mid orbit (59 nodes):** Plane OR island confirmed, OR sustained post-conviction contact, OR postconv+financial relationship, OR direct legal involvement. Rendered at 1.2× base size, ~185px from centre. Includes Trump, Clinton, Bannon, Gates, Hoffman, Brin, Branson, Mandelson, Chopra, Attia, Siegal, Tisch, Mette-Marit, Sulayem and others.
- **Tier 3 — Peripheral (36 nodes):** Social access, single events, correspondence only. Rendered at 0.95× base size, ~290px from centre. Includes Oz, Feinberg, Musk, Zuckerberg, Boehly, Lavrov, Previn, Dawkins, Briatore and others.

**D3 physics updated:** Link distances and strengths weighted by tier. Charge repulsion also tier-scaled so inner nodes cluster more tightly.

**Editorial overrides applied:** Several nodes moved from Tier 3 to Tier 2 after review — Chopra (dozen post-conviction meetings, publicly defended Epstein), Attia (1,700+ file references, "can't tell a soul" email), Siegal (post-conviction social rehabilitation node), Mette-Marit (close 2011–2014 friendship, Palm Beach stays), Tisch (400+ references), Gelernter, Kosslyn.

### New: Proximity legend
Collapsible "Proximity key ▾" toggle added to the toolbar. Shows three labelled circles explaining tier meaning. Closed by default, expands inline.

### New: About modal
"About" button added to nav bar (right-aligned). Opens a modal with the project's curatorial statement and a warm acknowledgment of Epstein Exposed. Click outside or × to close.

> *"The Island Ledger is a curatorial project — not a research database. It exists to make 120+ documented connections legible at a glance: who was involved, what sector they operated in, and whether anyone faced consequences. Every entry is sourced to primary documents.*
>
> *If you want to go deeper into the raw record — 2.1 million searchable documents, 1,713 persons, full flight logs, and original EFTA filings — the best resource available is Epstein Exposed, a remarkable one-person public interest project that has done extraordinary work making the primary sources accessible. I use it. I recommend it without reservation.*
>
> *— Elena / Cyramatique"*

### New: Epstein Exposed links in every dossier panel
Every dossier now has two outbound research links:
- **Search Epstein Exposed ↗** — links directly to the person's profile page on epsteinexposed.com
- **Search in DOJ files ↗** — existing Pinpoint link (unchanged)

### Travel data audit — 82 nodes updated
Full cross-reference against confirmed reporting (CNN Mar 2026, Wikipedia Little Saint James, Bloomberg FCA filings, court records). Replaced 'unclear' with sourced values for 82 nodes.

**Key corrections:**
- Staley: island → `true` (FCA tribunal: stayed on island 2005/6 and 2009)
- Summers: island → `true` (CNN: spent less than a day on island on honeymoon 2005)
- Black: island → `true` (CNN: "picnic lunch" with family)
- Branson: island → `true` (CNN: toured island 90 mins 2013 — his own boat)
- Mandelson: island → `true` (CNN: spent 1–2 nights)
- Brin: island → `true` (CNN: spent a day with fiancée Wojcicki)
- Barak: island → `true` (Wikipedia: multiple visits 2014–2015)
- Wexner: island → `true` (congressional deposition Feb 2026)
- Pritzker: island → `true` (emails documented in CNBC Feb 2026)
- Krauss: island → `true` (organised 2006 island physics conference)
- 50+ peripheral figures: both set to `false` (confirmed correspondence/meetings only)

**Editorial note:** Island = Little Saint James only. Zorro Ranch (New Mexico) visits for Horner, Boyden, Staley treated separately — only Little Saint James counts as island `true`.

### CSV updated
- New `proximity_tier` column added (column 7)
- All travel data updated to reflect audit
- 124 rows, 11 columns

