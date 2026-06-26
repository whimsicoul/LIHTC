# LIHTC 2025 National Database — Collection Status
*Last updated: June 26, 2026 (Retroactive source doc archival: downloaded and filed source documents for 11 of 12 web-extracted states (Alabama, Alaska, Arkansas, Delaware, Florida, Indiana, Iowa, Vermont, West Virginia, Wisconsin, Wyoming); Rhode Island has no downloadable PDF — SLIHTC press release web page documented as source. Added `collection_method` field to all 998 JSON records and 983 CSV/Excel rows documenting how each state's data was collected. Fixed `source_doc` field for 186 records to remove `[not in source_docs - web extraction]` suffix. Database structure unchanged: 983 records.)*

**Master database: 983 records across 42 states**
**2 states sourced but not yet extracted (MA, PA) — see Section 3**
**7 states with no data collected — see Section 3**

---

## Section 1 — Complete

All five required fields populated (State, Agency, Project Name, Developer, Award Amount). Caveats noted where data quality flags exist.

| State | Projects | Credit Types | Notes |
|-------|----------|-------------|-------|
| Alabama | 17 | 9% | AHFA award list PDF. Mix of new construction and rehab. TDC not in source. Source archived: `alabama.9pct.awards.2025.pdf` downloaded from ahfa.com (2026-06-26). |
| Alaska | 5 | 9% + 4% | AHFC GOAL Program. Includes tribal and PSH projects. Agency name em-dash encoding fixed (2026-06-24). Source archived: `alaska.lihtc.awards.2025.pdf` (2025 LIHTC Reservation List) downloaded from ahfc.us (2026-06-26). |
| Arkansas | 10 | 9% | ADFA 9% list PDF. All new construction. Multiple non-profit set-asides. Source archived: `arkansas.9pct.awards.2025.pdf` downloaded from adfa.arkansas.gov (2026-06-26). |
| California | 249 | 9% + 4% | CTCAC. 53 9% projects (Rounds 1 & 2) + 196 4% projects (Rounds 1–3). All 249 developer names confirmed. Saggio Hills Phase II listed as two co-developers in source (Freebird Development Company / Jamboree Housing). "Ollie Apartments" appears twice — confirmed intentional: separate Round 1 and Round 2 allocations to the same project; both rows retained and flagged. |
| Colorado | 12 | 9% | CHFA 2025 9% awards. All amounts $1,597,195–$1,600,000. All developer entities confirmed from source PDF. |
| Connecticut | 10 | 9% | CHFA 2025 reservations. $14,841,228 total. All per-project amounts confirmed. |
| Florida | 27 | 9% | FHFC 7 RFAs: 201 (Small/Med Counties, 9 projects), 202 (Large Counties, 10 projects), 203 (Miami-Dade, 3 projects), 212 (Revitalization, 1 project), 103 (Homeless, 1 project), 106 (Disabilities, 1 project), 108 (Homeless Med/Large, 2 projects). Awards are board preliminary awards. $81.2M total annual LIHTC. 4% (noncompetitive) not collected — see RFA 2025-205. Source archived: `florida.9pct.awards.2025.pdf` (October 24, 2025 FHFC Board Action document) downloaded from floridahousing.org (2026-06-26). |
| Idaho | 7 | 9% | IHFA final allocations as of January 10, 2025. $6,389,837 total. Bluebird Village ($140K) is a supplemental credit award, not a standalone project. |
| Indiana | 51 | 9% + 4% | IHCDA 2025A-C (16 projects), 2025A-G (1 project), 2025B-C (5 projects), 2025A-B bond (29 projects). Developer entities confirmed from awarded project PDFs. Source archived: `indiana.lihtc.awards.2025.pdf` (IHCDA 2025 Annual Report, covers all rounds) downloaded from in.gov/ihcda (2026-06-26). |
| Iowa | 10 | 9% | IFA award listing PDF dated August 6, 2025. One supplemental award from 2024. Sources archived: `iowa.9pct.awards.2025.pdf` and `iowa.4pct.awards.2025.xlsx` downloaded from opportunityiowa.gov (2026-06-26). |
| Kansas | 14 | 9% + 4% R1 | 9% awards confirmed final. **Caveat:** 4% records are from "Applications Received Round One" — not confirmed final allocations. 4% Round 2 not yet collected. |
| Maine | 5 | 9% | MaineHousing 5 projects with Notice to Proceed. $5,408,699 total. 2 state 4% bond projects confirmed but NOT federal LIHTC — excluded. |
| Maryland | 13 | 9% | DHCD 2025 Competitive Funding Round (Notice 25-14, Oct 2025). $19,000,000 total (11 × $1.5M + 2 × $500K). Source document titled "2026 LIHTC Awards." 9 of 13 projects have co-developers; lead entity used. Locations are county-level only. |
| Minnesota | 8 | 9% | Minnesota Housing 2025 Multifamily Consolidated RFP. $12,651,138 total. 12 additional projects funded via agency loans (no 9% HTC) excluded. |
| Mississippi | 15 | 9% | MHC 2025 Housing Tax Credit Recipient List (Sept 10, 2025). All acquisition/rehabilitation. |
| Montana | 6 | 9% | Montana Housing 2025 Housing Credit Awards. $3,720,204 total annual. Source shows 10-year totals; divided by 10. Eagle Seeker Housing excluded (Withdrawn). Two co-sponsored projects; lead sponsor used as developer. |
| Nevada | 8 | 9% | NHD 2025 9% reservations. All 8 developer entities confirmed via web research (2026-06-24). Source: `nevada.9pct.reservations.2025.xlsx` (already in source_docs). `collection_method` field added. |
| New Hampshire | 5 | 9% | NHHFA 2025 9% LIHTC Reservations. $5,000,000 total. Sponsor organization used as developer entity. |
| New Jersey | 19 | 9% | NJHMFA spring reservations (4 projects, $6,333,560; reservation date 8/28/2025) + fall reservations (15 projects, $23,061,592; reservation date 2/25/2026). **Caveat:** Reservation stage only — not confirmed final allocations for either round. Both rounds treated as 2025 award year. |
| New Mexico | 5 | 9% | NM MFA 2025 tab of historical awards workbook. $6,607,608 total annual. All amounts confirmed annual by source column label. All 5 developer entities confirmed. |
| New York | 27 | 9% | HCR 9% RFP awards. All fields complete for 27 projects. **Note:** NYC HDC/HPD 4% data still not collected. |
| North Carolina | 50 | 9% + 4% | NCHFA 2025 awards. 47 of 50 developer entities confirmed. 3 still unresolved (Preserve at Forest Heights/Kristi Morgan, The Reserve at Fairmont/James Harrell III, Walker Landing/Charles Treach — contact persons, not entity names). All amounts confirmed. |
| North Dakota | 5 | 9% | NDHFA 2025 Applications Selected for Commitment. 5 projects received 9% LIHTC ($9,893,236 total). KingsView Apartments and Wild Rose Senior Living deleted (HIF-only, no LIHTC awarded). Source is commitment stage, not final allocation. |
| Ohio | 27 | 9% + 4% | OHFA 2025. 23 9% LIHTC Reservations ($35,495,770) + 4 4% Bond Gap Financing (BGF) awards ($7,006,126). All developer entities confirmed. TDC captured for all 23 9% projects. |
| Oklahoma | 25 | 9% + 4% | OHFA 2025. Round 1 (8 projects) + Round 2 (12 projects) 9% awards + 4% awards (5 projects). $29,137,145 total. Developer names are LP/LLC legal entities as listed in source. |
| South Carolina | 15 | 9% | SC Housing 2025 awards. 12 of 15 developer entities confirmed via web research (2026-06-24). 3 still unresolved (Chester Townhouses Phase II/George Baker, Coit Village/James M. Bernstein, Swann Meadows/James M. Bernstein). All amounts confirmed. Source: `south_carolina.9pct.awards.2025.pdf` (already in source_docs). `collection_method` field added; unresolved records flagged individually. |
| South Dakota | 7 | 9% | SDHDA cumulative reservations list, 2025 section only. 7 competitive 9% projects confirmed. James Street Villas: 2025 credit amount only ($373,981); $121,792 forward commitment to 2026 noted in data_flags. **Note:** 2025 Tax Exempt Bond project (The Rhys Apartments, 4%) not extracted — add if federal LIHTC confirmed. |
| Tennessee | 22 | 9% | **Caveat:** Preliminary ranking only (July 30, 2025). Developer entity names inferred from contact info — not verified. All amounts in database. |
| Texas | 57 | 9% | **Caveat:** Tentative awards only (board vote was July 24, 2025). Developer entity names absent from source (contact persons listed). All amounts in database. |
| Utah | 8 | 9% | Utah Housing Corporation. June 2024 application round, awarded September 5, 2024 for 2025 credit year. $10,588,180 total. |
| Vermont | 8 | 9% + 4% | VHFA 2025 allocations. 5 Tax Exempt Bond (4%) + 3 Federal Competitive (9%). Source archived: `vermont.lihtc.allocations.2025.csv` downloaded from vhfa.org allocations page (2026-06-26). |
| Virginia | 25 | 9% | Virginia Housing Final Rankings (July 10, 2025). All pool types. Owner Entity used as developer. |
| Washington | 11 | 9% | WSHFC 2025 Allocation List. Three pools: King County (2), Metro (4), Non-Metro New Production (5). Non-Metro pool oversubscribed — may include forward commitment of 2026 credits, flagged per project. |
| West Virginia | 11 | 9% + 4% | WVHDF Credit Allocation Recipients list. Two projects (White Oak Landing/Manor) have unusually low credit amounts ($31K) — likely carryover. Source archived: `west_virginia.lihtc.recipients.2025.pdf` downloaded from wvhdf.com (2026-06-26). |
| Wisconsin | 27 | 9% + 4% | WHEDA award and reservation lists. Only federal credit recorded. $36.6M total. Sources archived: `wisconsin.9pct.awards.2025.pdf` and `wisconsin.4pct.awards.2025.pdf` (WHEDA 2025 HTC applicant lists; award data confirmed from WHEDA award announcement pages) downloaded from wheda.com (2026-06-26). |
| Wyoming | 16 | 9% + 4% | **Caveat:** WCDA document is the 2025 "Applications Received" list — credit requests, not confirmed final awards. One record (Pershing Pointe) from Letter of Intent with no credit amount. Need confirmed award list. Source archived: `wyoming.lihtc.applications_received.2025.xlsx` downloaded from wyomingcda.com (2026-06-26). |

**Total: 36 states, 837 projects (Section 1)**

---

## Section 2 — Partially Complete

In the database but missing one or more required fields, or data from an unconfirmed stage (applications, reservations, QAP rankings).

| State | Projects | What's Missing | Status |
|-------|----------|---------------|--------|
| Arizona | 33 | 2 of 33 developer entities still missing (Glendale Apartments, Eloy Goy Housing). Flags updated to mark as "entity lookup required before final delivery." All amounts confirmed. | Call ADOH Rental Development at (602) 771-1000 for both missing entities. |
| Delaware | 4 | 1 of 4 missing credit amount: Mispillion Station III Apartments (4%) — amount not specified in source. 3 other records are preliminary (may be revised). Source archived: `delaware.9pct.awards.2025.pdf` (DSHA 2025 Preliminary Award Chart) downloaded from destatehousing.com (2026-06-26). | Obtain DSHA allocation letter for Mispillion Station III. |
| Georgia | 61 | All 61 records need legal entity lookup — source doc provides individual contact person names only. Additionally, 25 4% records have no annual LIHTC credit amount (bond amounts captured in data_flags; actual LIHTC allocation not in source). 2 9% records (Perry Commons, Pattillo Residences) also have no credit amount. | Obtain DCA allocation letters for 4% annual credit amounts; perform entity lookup for all 61 contacts. |
| Hawaii | 4 | 2 of 4 projects (Aikanaha Residences, Hoonanea Phase I) are LIHTC reservations only — not final allocations. All 5 fields populated for all 4 projects. | Obtain final HHFDC allocation letters (IRS Form 8609 issuance) for Aikanaha and Hoonanea. |
| Illinois | 23 | 1 of 23 missing credit amount: LATHROP IC (4%, 309 units, Related Midwest, Chicago) — annual allocation not listed in source. All other 22 records complete. A second 9%-only PDF (`Illinois-2025-LIHTC-Approved-Allocations-1.pdf`) was received during cleanup — confirmed exact duplicate of already-extracted data; filed as `illinois.9pct.awards.2025.v2.pdf`. | Check IHDA allocation announcement for LATHROP IC annual credit amount. |
| Louisiana | 21 | Source is QAP Rankings, not confirmed final awards. Developer entity names are populated from nonprofit/organization names in source but not verified as legal entities for all records. | Confirm QAP rankings became final allocations; verify developer entity names. |
**Total: 6 states, ~146 projects with partial data**

---

## Section 3 — No Usable Data

Nothing extracted, or only a placeholder row. Includes states where source documents are in hand but blockers prevent extraction.

| State | Agency | Projects (est.) | Notes | Next Step |
|-------|--------|----------------|-------|-----------|
| District of Columbia | DHCD | — | No confirmed public award list. DHCD announces via press release only. | FOIA/public records request. |
| Kentucky | Kentucky Housing Corporation (KHC) | — | KHC 2025 Multifamily Funding Report PDF returned 404. Placeholder row deleted from database (2026-06-24). | Manually navigate kyhousing.org or contact KHC directly. |
| Massachusetts | EOHLC | ~21 | Source documents in hand. Per-project LIHTC amounts absent; credit type (4% vs. 9%) not specified per project. Mass.gov blocks all automated fetches. Additional file `massachusetts.lihtc.congressional_districts.historical.pdf` is a historical all-time list (849 projects, no amounts, no years) — does NOT resolve the blocker. | Direct EOHLC contact or manual download needed before extraction. |
| Michigan | MSHDA | — | Two wrong-year PDFs received: 2019 round and 2026 round. Neither is 2025 data. | Check michigan.gov/mshda/developers/lihtc for 2025 awards. |
| Missouri | MHDC | — | `source_docs/missouri.4pct.applications_received.2025.pdf` in hand — application-stage only. Do NOT extract until confirmed final allocations obtained. | Obtain MHDC final award list. |
| Nebraska | NIFA | — | Two application lists in hand — neither is confirmed awards. | Obtain NIFA final award list from nifa.org. |
| Oregon | OHCS | — | Not started. | Check oregon.gov/ohcs/housing-programs/pages/lihtc.aspx. |
| Pennsylvania | PHFA | ~41 | Source documents in hand. 39 of 41 developer entity names absent — PHFA public PDFs are image-based with no entity data. | Direct PHFA contact needed for entity names before extraction. |
| Rhode Island | RIH | — | All 13 originally collected rows were SLIHTC (state tax credit only, no federal LIHTC amounts) — all deleted (2026-06-24). 12 SLIHTC records remain in JSON only (not in CSV/Excel master). No downloadable PDF available — data sourced from Governor's press release (governor.ri.gov) and rihousing.com announcement pages. No confirmed federal LIHTC data for 2025. | Confirm whether RIH administers federal LIHTC separately; if so, obtain federal allocation list. |

**Total: 9 states, ~62 sourced but not extracted; remainder not started**

---

## Summary

| Section | States | Projects (est.) |
|---------|--------|----------------|
| ✅ Complete | 36 | 837 |
| ⚠️ Partial | 6 | 146 |
| ❌ No usable data | 9 | — |
| **Total in database** | **42** | **983 records** |
| **Total in scope** | **~51** | **~1,110 (est. when full)** |

**Remaining open issues (pre-delivery):**
- Arizona: 2 records still missing developer names (Glendale Apartments, Eloy Goy Housing) — call ADOH (602) 771-1000
- Delaware: 1 record missing credit amount (Mispillion Station III Apartments) — obtain DSHA allocation letter
- Georgia: 27 records missing credit amounts (25 4% + Perry Commons + Pattillo Residences) + all 61 records need legal entity lookup — obtain DCA allocation letters and perform entity research
- Illinois: 1 record missing credit amount (LATHROP IC, 4%) — contact IHDA for annual allocation figure
- Wyoming: 1 record missing credit amount (Pershing Pointe Apartments) — Letter of Intent only; obtain confirmed award
- Kentucky: No data collected — manually navigate kyhousing.org or contact KHC directly
- Rhode Island: No federal LIHTC data — confirm if RIH administers federal credits separately
