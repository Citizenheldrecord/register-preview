# Citizen Held Record register: design test copy

This folder is a local preview of a redesigned public register. It is not the live site.

- Do not push this folder to Citizenheldrecord/register or to any public remote.
- Do not upload it. Do not run tools/ship.py from here.
- The live site, its repo, its data file and its URLs were not changed.
- The page reads `data/entries.csv` with the live schema unchanged, so a later drop-in would not need data changes.

To view it locally:

    python3 -m http.server 8765
    # then open http://127.0.0.1:8765/

Screenshots are in `screenshots/`.
