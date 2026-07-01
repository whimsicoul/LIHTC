# LIHTC 2025 National Database — Collection Status
*Last updated: July 1, 2026*

**Master database: 1,112 records across 46 states**
**JSON note:** `lihtc_data/all_states.lihtc.2025.json` has 1,125 records (48 states/territories) — 13 more than the CSV/Excel master. Kentucky (1 placeholder, no real data) and Rhode Island (12 rows, state tax credit not federal LIHTC) are excluded from the master per CLAUDE.md's five-field rule but kept in JSON.

**Columns beyond the core five:**
- `source_count` — number of distinct source docs backing a row
- `award_status` — `Final` or `Preliminary`, based on source language (reservation/application-stage vs. confirmed award). 55 of 1,020 records (5.6%) are Preliminary.

---

## Section 1 — Complete
All five required fields populated. Caveats noted where relevant.

| State | Projects | Credit Types | Notes |
|-------|----------|-------------|-------|
| Alabama | 17 | 9% | AHFA award list. |
| Alaska | 5 | 9% + 4% | AHFC GOAL Program; includes tribal/PSH projects. |
| Arkansas | 10 | 9% | ADFA award list. |
| California | 249 | 9% + 4% | CTCAC, Rounds 1–3. "Ollie Apartments" appears twice intentionally (separate Round 1/2 allocations). |
| Colorado | 12 | 9% | CHFA 2025 awards. |
| Connecticut | 10 | 9% | CHFA 2025 reservations, $14.8M total. |
| Florida | 27 | 9% | FHFC board "tentative selection" awards across 7 RFAs, $81.2M total. 4% not collected. |
| Idaho | 7 | 9% | IHFA final allocations, $6.4M total. |
| Indiana | 78 | 9% + 4% | IHCDA/READI 2.0 awards across multiple 2025/2026-labeled rounds. Sourced via web research (agency doesn't publish a single consolidated list); `source_doc` flagged accordingly. |
| Iowa | 14 | 9% + 4% | IFA award lists (Aug 2025 9%, June 2026 4%). |
| Kansas | 22 | 9% + 4% | 9% confirmed final. 4% (8 projects): no per-project dollar amounts published by KHRC — flagged. |
| Louisiana | 21 | 9% | LHC Final Rankings (Oct 2025), $14.8M total. |
| Maine | 5 | 9% | MaineHousing, $5.4M total. |
| Maryland | 13 | 9% | DHCD 2025 round, $19M total. |
| Minnesota | 8 | 9% | Minnesota Housing Consolidated RFP, $12.7M total. |
| Mississippi | 15 | 9% | MHC 2025 recipient list. |
| Missouri | 45 | 9% + 4% | MHDC 2025 board-approved awards (31 in the 9% list, some rows drawing 4% credit; 14 more from a separate 4% approvals list), $50.8M total. |
| Montana | 6 | 9% | Montana Housing, $3.7M annual total. |
| Nebraska | 12 | 9% | NIFA 2025 Reservations list (12/17/2025), $6.7M total. Reservation stage — no separate final-allocation document found; flagged Preliminary. |
| Nevada | 8 | 9% | NHD 2025 reservations. |
| New Hampshire | 5 | 9% | NHHFA reservations (agency's operative award terminology), $5M total. |
| New Jersey | 19 | 9% | Spring + fall reservations, $29.4M total. Reservation stage only — no public data on which have converted to final allocations. |
| New Mexico | 5 | 9% | NM MFA 2025 awards, $6.6M total. |
| New York | 27 | 9% | HCR 9% RFP awards. NYC HDC/HPD 4% not collected. |
| Oregon | 10 | 9% + 4% | OHCS Oct 2025 awards; 3 projects are reservations pending final allocation. |
| North Carolina | 50 | 9% + 4% | NCHFA 2025 awards. 1 developer entity unresolved (The Reserve at Fairmont). |
| North Dakota | 5 | 9% + 4% | NDHFA 2025 commitments, $9.9M total. |
| Ohio | 27 | 9% + 4% | OHFA reservations + Bond Gap Financing awards, $42.5M total. |
| Oklahoma | 25 | 9% + 4% | OHFA 2025, $29.1M total. |
| South Carolina | 15 | 9% | SC Housing 2025 awards. 2 developer entities unresolved (Chester Townhouses II, Coit Village). |
| South Dakota | 7 | 9% | SDHDA 2025 reservations. |
| Tennessee | 18 | 9% | THDA preliminary ranking, confirmed final via press release. Developer names are orgs, not legal entities. |
| Utah | 8 | 9% | Utah Housing Corp, $10.6M total. |
| Vermont | 8 | 9% + 4% | VHFA 2025 allocations. |
| Virginia | 25 | 9% | Virginia Housing Final Rankings (July 2025). |
| Washington | 11 | 9% | WSHFC 2025 allocations; Non-Metro pool may include 2026 forward-committed credits. |
| West Virginia | 11 | 9% + 4% | WVHDF recipients list. |
| Wisconsin | 27 | 9% + 4% | WHEDA award/reservation lists, $36.6M total. |
| Wyoming | 4 | 9% | WCDA official awards-by-year list. |

**Total: 39 states, 891 projects**

---

## Section 2 — Partially Complete
In the database but missing one or more required fields, or unconfirmed-stage data.

| State | Projects | What's Missing | Next Step |
|-------|----------|---------------|-----------|
| Arizona | 33 | 2 developer entities missing (Glendale Apartments, Eloy Goy Housing). | Call ADOH Rental Development (602) 771-1000. |
| Delaware | 4 | 1 missing credit amount (Mispillion Station III); 3 records preliminary. **Re-checked (2026-07-01):** no finalized award chart or board minutes with per-project figures found beyond what was already known — dead end via web search. | Obtain DSHA allocation letter. |
| Georgia | 59 | 25 of 59 (the 4% projects) missing annual LIHTC credit amount — DCA only publishes bond amount, confirmed non-disclosure not an extraction gap. | Obtain DCA 4% allocation letters if needed. |
| Hawaii | 4 | 2 projects (Aikanaha, Hoonanea Phase I) are reservations, not final allocations. | Obtain final HHFDC allocation letters. |
| Illinois | 23 | 1 missing credit amount (LATHROP IC, 4%) — not published at per-project level. | Contact IHDA. |
| Michigan | 35 | MSHDA's Jan 29, 2025 press release states 15 projects/$17.3M total but only itemizes 12 by name/amount; the other 3 projects (~$2M) aren't extractable without guessing. All 35 records are confirmed final 9% awards across 3 rounds (Jan, Jul, Dec 2025). | Check if MSHDA published a fuller list/PDF for the Jan 29 round covering the 3 missing projects. |
| Texas | 63 | 1 developer name missing (Pathways at Santa Rita Courts West — assigned to an individual, no company in source). | Contact TDHCA/HACA directly. |

**Total: 7 states, 221 projects**

---

## Section 3 — No Usable Data
Nothing extracted, or only a placeholder row.

| State | Agency | Notes | Next Step |
|-------|--------|-------|-----------|
| District of Columbia | DHCD | No public award list; press-release only. | FOIA/public records request. |
| Kentucky | KHC | Website migration broke the 2025 report link; no replacement found. | Call KHC Multifamily (800) 633-8896 or multifamily@kyhousing.org. |
| Massachusetts | EOHLC | Source docs in hand; per-project amounts and credit type absent. Mass.gov blocks automated fetches. | Direct EOHLC contact or manual download. |
| Pennsylvania | PHFA | Source docs in hand; image-based PDFs, no entity data for 39 of ~41 projects. | Direct PHFA contact needed. |
| Rhode Island | RIH | Only state tax credit (SLIHTC) data found, no federal LIHTC. | Confirm if RIH administers federal LIHTC separately. |

**Total: 5 states, ~62 projects sourced but not extracted (or not applicable); remainder not started**

---

## Summary

| Section | States | Projects |
|---------|--------|----------|
| ✅ Complete | 39 | 891 |
| ⚠️ Partial | 7 | 221 |
| ❌ No usable data | 5 | — |
| **Total in database** | **46** | **1,112 records** |
| **Total in scope** | **~51** | **~1,235 (est. when full)** |

**2026-07-01 web-research pass:** Targeted follow-up search on the 4 states/gaps most likely to have a findable update (Michigan, Missouri, Nebraska, Delaware). Michigan went from zero data to 35 confirmed final 9% awards (3 MSHDA press releases). Missouri went from application-stage-only to 45 confirmed board-approved awards (2 MHDC PDFs). Nebraska went from application-stage-only to 12 confirmed reservations (NIFA list, flagged Preliminary — not yet final allocation). Delaware's Mispillion Station III amount remains unresolved; no newer source found, confirmed dead end for now.
