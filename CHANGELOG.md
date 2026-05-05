# Changelog — The Island Ledger

All notable changes to this project are documented here.
Format: [version] — date · description

---

## [v1.8] — 2026-05-05

### Network diagram — epstein-network-individuals.csv

- **Added: Naomi Campbell** (`id: naomi`, sector: social, status: named, r: 11)
  - Plane travel flagged true; island: unclear
  - Sources: EFTA corpus · FBI Prominent Names briefing (Jan 30 2026 release) · flight logs (Epstein Flight Explorer) · The Guardian · BBC
  - Dossier notes: appears in Epstein's released contact book; listed in FBI Prominent Names briefing; social connection via Ghislaine Maxwell documented; not accused of wrongdoing, no charges filed
- **Network count: 125 nodes** (124 individuals + Epstein as centre)
- Updated `epstein-network-individuals.csv` to reflect addition

---

## [v1.7] — 2026-04-25

### Network diagram

- Added: Pam Bondi (status: removed — fired Apr 2 2026)
- Added: Melania Trump (status: named — EFTA02332411 email authenticated)
- Added: Kevin Warsh, Brett Ratner, David Hanson, John de Jongh Jr., Lawrence Delson, Steve Tisch, Tsakhiagiin Elbegdorj, Soon-Yi Previn
- Status updates: Tom Pritzker, Dean Kamen → stripped; Brad Karp, Robert Trivers → fuller documentation
- Cleaned duplicate/placeholder nodes; network stabilised at 122 → 124 nodes across prior patch
- 48 clickable name links wired to inline mini-dossier panel
- Sticky sidebar, live proceedings status chips, EFTA document reference chips

### Timeline (timeline.html)

- Breaking news entry added: Pam Bondi firing Apr 2 2026 (timeline only — no direct documented Epstein connection)

---

## [v1.6] — 2026-04-10

### Timeline (timeline.html)

- Full rebuild of Trump Timeline view
- Four tabs: The Epstein Files · An Illegal War · The Money · Legal Track
- Format A (evidence table) for Legal Track
- Format B (claim/counterclaim) for Epstein Files and Iran
- Format C (timestamped ledger) for The Money
- 74 total records across all tabs
- 7 flight log links wired to Epstein Flight Explorer (imanebayoub.github.io/Epstein-Flight-Explorer)
- Badge system across 14 source types
- Consolidated full dataset: island_ledger_full_dataset.csv (74 rows, 9 columns)

### Network diagram

- D3 force-directed diagram replaced on mobile with searchable tap-to-expand list
- Google Analytics integration (showPage() event tracking)

---

## [v1.5] — 2026-03-20

### Network diagram

- 9 new individuals added (sourced via Wikipedia Epstein files list and EFTA cross-reference)
- EFTA document reference chips added to dossier panel
- Source methodology: Google Pinpoint deep links for dossier entries
- EFTA document numbers established as primary citation format

---

## [v1.0] — 2026-02-01

### Initial release

- 121-node force-directed D3.js network (120 individuals + Epstein as centre)
- Mar-a-Lago luxury visual theme: Playfair Display, Cormorant Garamond, Cormorant SC
- Parchment / hunter green / aged gold palette
- Supporting data: epstein-accusations.csv
- GitHub Pages deployment: cyramatique.github.io/TheIslandLedger/
