# FAILED entry fields: <ENTRY-ID>

Template for the five mandatory fields on a FAILED register entry (draft rule, 27 Oct 2026; wording awaits Barry's approval).
Copy to sources/failed/<ENTRY-ID>.md, where <ENTRY-ID> is the frozen *-SCORED-YYYYMMDD id in data/entries.csv.

Fill-once: the entry in data/entries.csv is never edited. This file is append-only. Each update is a NEW dated line
below the last one; never edit or remove an earlier line. A later line may add or update a field; the check reads all lines.
A value of TBD, READ PENDING, none, - or n/a does not count.

## Line YYYY-MM-DD
- 1. Required / record on scoring date: <what the test required, and what the record showed on the scoring date, with the URL read>
- 2. Why still live: <why the commitment or failure still matters: not withdrawn, still promised, deadline moved, etc.>
- 3. Accountable: <the holder who can close it (minister, office, body, party), not the desk that records it>
- 4. Closing document or promise: <quoted line from the holder's own source, with its URL and read date (CST)> OR "none on record as of <date> (searched: <URLs>)"
- 5. Next check: <YYYY-MM-DD> plus either a follow-up row ID in data/entries.csv or "quarterly recheck"
  From 2026-11-13 (RULEBOOK R3.12, Barry t3408u, t3409u, go t3410s16560; forward-only, earlier FAILED scores are not reopened):
  field 5 also names either the proposed follow-on row (an id live or in reports/CANDIDATES.md, given to
  tools/add_entry_checked.py score --follow-on ID) or the line "no dated next step found; late watch until <YYYY-MM-DD>",
  12 months after the scoring date (score --late-watch, which writes the desk LATE-WATCH.csv line).
  If the PASS condition later appears on a primary, it is a new DELIVERED LATE row (R3.11, tools/add_entry_checked.py late),
  following the original promise id; this FAILED entry and its count are never changed.
