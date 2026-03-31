# The Island Ledger \& The Resident Representatives

### An interactive investigation into the Epstein files

**Designed by** [**Cyramatique**](https://www.yourlocalanthropologist.com)  
A project by Elena Walton · *Your Local Anthropologist*

\---

## What this is

A self-contained interactive HTML investigation mapping 122 documented individuals in the Jeffrey Epstein files, cross-referenced against the DOJ's public EFTA document release. Built for journalists, researchers, and the public as a navigable reference — not a client list, not speculation. Every entry is sourced.

Two views. One file. No server required.

\---

## Files in this repository

|File|Description|
|-|-|
|`index.html`|**Main deliverable.** Two-page interactive investigation — open in any browser|
|`database.csv`|Structured data: 122 individuals with sector, status, travel record, connection summary, consequence, and source citations|
|`README.md`|This file|
|`CHANGELOG.md`|Dated log of all additions and updates|

\---

## How to use

Open `epstein-unified.html` in any modern browser. Switch between pages using the navigation bar at the top.

### The Island Ledger — network diagram

* **Click any node** to open a dossier panel with connection summary, consequence status, travel record, and a direct link into the DOJ Pinpoint archive
* **Filter by status** (Removed / Stripped / Active / Deceased / Pending / Incarcerated) or **by sector** using the toolbar chips
* **Search by name** to highlight individuals
* **Drag** to reposition nodes · **scroll** to zoom

### The Resident Representatives — three-track timeline

Three tracks covering the administration's handling of the files:

* **Timeline** — 20 entries documenting the administration's narrative and reversals
* **Legal Track** — 10 proceedings across civil litigation, congressional oversight, and criminal/judicial
* **Document Record** — 8 official claims cross-referenced against specific EFTA document numbers

\---

## Status categories

|Status|Colour|Meaning|
|-|-|-|
|Removed|Crimson|Resigned, fired, or removed from position as a direct consequence|
|Stripped|Amber|Sanctioned, fined, title stripped, or stepped down under pressure|
|Active|Navy|No formal action taken as of last update|
|Deceased|Green|Died — before or after file release|
|Pending|Purple|Under criminal investigation or facing charges|
|Incarcerated|Black|Currently serving a prison sentence|

\---

## Sectors

|Sector|Description|
|-|-|
|Political|Heads of state, ministers, diplomats, current administration officials|
|Finance|Private equity, banking, hedge funds, real estate|
|Tech / Science|Silicon Valley, academia, research funding networks|
|Legal / Enabler|Attorneys, co-conspirators, operational associates|
|Social / Cultural|Media, entertainment, royalty, social access nodes|

\---

## The CSV

`epstein-accusations.csv` — 10 columns, 122 rows, one per individual in the diagram.

|Column|Description|
|-|-|
|`name`|Full name|
|`title`|Role / affiliation|
|`sector`|political / finance / tech / legal / social / center|
|`status`|active / removed / stripped / pending / deceased / incarcerated|
|`plane`|true / false / unclear / claimed\_never|
|`island`|true / false / unclear / claimed\_never|
|`connection\_summary`|Documented connection to Epstein (truncated to 300 chars)|
|`consequence`|Current status and any formal actions|
|`badges`|Connection types: financial / social / legal / alleged / access / postconv / enabler|
|`source`|Primary source citations|

The CSV is version-controlled — every status change is traceable in git history.

\---

## Sources

All entries sourced to at least one of:

* **DOJ Epstein Library** — `justice.gov/epstein`
* **EFTA document numbers** — cited per dossier (e.g. EFTA01656152)
* **Google Pinpoint / Courier Newsroom** — `journaliststudio.google.com/pinpoint/search?collection=c109fa8e7dcf42c1` (requires Google account)
* **rhowardstone/Epstein-research** — forensic analysis of the 218GB corpus
* **Wikipedia: List of people named in the Epstein files**
* **Democracy Defenders Fund** — `democracydefendersfund.org/epstein-files`
* Contemporary reporting: NPR, NBC News, CNN, Al Jazeera, Britannica, Inside Higher Ed, Scientific American, Reuters, Times Higher Education

\---

## Editorial policy

**Appearing in this diagram does not mean a person committed a crime.**

The DOJ itself notes that names appear in the files in a wide variety of contexts — from direct email correspondence to incidental mentions in news clippings. We follow the same standard: documented, sourced connection to Epstein or the files. The dossier panel for each individual explains the nature and depth of that connection.

Where allegations are unverified or disputed, this is stated explicitly in the dossier. Where the DOJ has called specific documents fake (e.g. EFTA00025010), this is flagged prominently.

No entry has been added based on unverified social media claims, conspiracy theory sources, or the DOJ's politically exposed persons letter alone.

\---

## What this is not

* Not a "client list" — no such list has been found in the files
* Not an accusation of criminal conduct against anyone not charged or convicted
* Not affiliated with any political party, campaign, or advocacy organisation

\---

## Updates

This is a living document. The GAO investigation is ongoing, FBI 302s remain partially withheld, and congressional oversight continues. See `CHANGELOG.md` for a dated record of all changes.

To suggest a correction or flag a sourcing error, open an issue.

\---

## Technical

Built with [D3.js](https://d3js.org) · Fonts: Playfair Display, Cormorant Garamond, Cormorant SC via Google Fonts · No backend, no dependencies beyond a browser

*No advertisers. No sponsors. Independent research.*

\---

*Last updated: March 2026*

