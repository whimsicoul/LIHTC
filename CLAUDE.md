# LIHTC 2025 National Database — Project Instructions for Claude

## What This Project Is

This is a data collection and assembly project building a national database of 2025 Low-Income Housing Tax Credit (LIHTC) awards across all 50 U.S. states + DC. The end goal is a single clean table (delivered as CSV and Excel) that the user can show their boss, with exactly five columns:

| State | Agency Name | Project Name | Developer That Won the Award | Award Amount ($) |

No extra columns, no partial records — every row must have all five fields populated.

---

## My Role Each Session

When the user drops new source files into the **project root** (`c:\Users\qylga\Desktop\Projects\jb\`), I should:

1. **Detect new files** — any PDF, XLSX, or CSV sitting in the root (not in `source_docs/` or `lihtc_data/`) is a new file to process.
2. **Extract the five required fields** from the file:
   - State
   - Agency name (the state housing finance agency that issued the award)
   - Project name
   - Developer that won the award (legal entity name, not a contact person's name)
   - Award amount in dollars (annual federal LIHTC credit, not total project cost)
3. **Append the extracted records** to:
   - `lihtc_data/all_states.lihtc.2025.json` (or the relevant state JSON file)
   - `LIHTC_Master_Database_2025.xlsx` and `lihtc_master_2025.csv`
4. **Move the source file** into `source_docs/` using the naming convention: `{state}.{credit_type}.{doc_type}.{year}.{ext}` (e.g., `virginia.9pct.awards.2025.pdf`)
5. **Update `LIHTC_Collection_Status.md`** — move the state from its current section to the appropriate section, note any caveats (missing fields, application-stage vs. final awards, etc.), and update the summary counts at the bottom.

---

## File Locations

```
jb/                                      ← project root (drop new files here)
├── CLAUDE.md                            ← these instructions
├── LIHTC_Collection_Status.md           ← running status tracker (always update after work)
├── LIHTC_Master_Database_2025.xlsx      ← master Excel database
├── lihtc_master_2025.csv                ← CSV export of master database
├── source_docs/                         ← raw source documents (move files here after extraction)
└── lihtc_data/                          ← structured JSON per state or state group
    └── all_states.lihtc.2025.json       ← consolidated JSON across all states
```

---

## Data Quality Rules

- **Award amount** = annual federal LIHTC credit allocation in dollars. If a source shows 10-year totals, divide by 10. If a source is application-stage (not final awards), flag it with a caveat — do not present it as confirmed.
- **Developer name** = legal entity name. If the source only lists a contact person (not a company), flag it as needing entity lookup. Do not invent or guess entity names.
- **Credit type** = 9% (competitive) or 4% (noncompetitive/bond). Capture both where applicable.
- **Partial records are acceptable but must be flagged** — a missing developer name or credit amount gets a note in the status file, not a fake value.
- **Do not duplicate records** — check the master CSV before appending; if a project already exists for that state, update rather than add a second row.

---

## Caveats to Watch For

- Some states publish "applications received" or "QAP rankings" before final awards — these are **not** confirmed allocations. Always note this.
- Some states have two allocators (e.g., New York has HCR statewide + NYC HDC/HPD for NYC projects). Collect both.
- Some states publish 10-year credit totals — divide by 10 to get the annual amount.
- Developer names in some PDFs are contact person names, not legal entities. Flag these.

---

## Status File Format

After every extraction session, update `LIHTC_Collection_Status.md`:
- Move the state to the correct section (✅ complete, ⚠️ partial, ❌ blocked, ⏳ pending).
- Add a row to the table with project count, credit types, and a brief note on data quality.
- Update the **Summary Counts** table at the bottom.
- Add a timestamp line at the top: `*Last updated: {date}*`

---

## Current Database State (as of 2026-06-23)

- **621 records across 20 states** in `lihtc_master_2025.csv`
- States with complete data: AL, AK, AR, DE, GA, IL, IA, KS (9% only), MS, WV, WI, WY
- States with partial data: AZ (no developer/amounts), CA (4% R2+R3 not parsed, 9% missing developers), CO (no amounts), CT (no per-project amounts), IN (~41 missing amounts), LA (no developer entities), NY (NYC 4% not collected)
- Source docs in hand but not yet extracted: HI, ID, ME, MN, MO
- New files in root awaiting processing: `virginia-lihtc-final-rankings-2025-07102025.pdf`, `2texas-50718-HTC9pct-TentativeAwardWaitingList.xlsx`, `NewHampshire-Current-LIHTC-Reservations.pdf`

---

## Naming Conventions for source_docs/

Format: `{state_lowercase}.{credit_type}.{doc_type}.{year}.{ext}`

Examples:
- `virginia.9pct.awards.2025.pdf`
- `texas.9pct.tentative_awards.2025.xlsx`
- `new_hampshire.lihtc.reservations.2025.pdf`
- `california.4pct.awards.round2.2025.xlsx`

Credit type options: `9pct`, `4pct`, `lihtc` (use `lihtc` when the doc covers both or type is unknown)
Doc type options: `awards`, `allocations`, `reservations`, `recipients`, `tentative_awards`, `applications_received`, `qap_rankings`, `annual_report`
