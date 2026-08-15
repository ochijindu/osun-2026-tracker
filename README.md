# osun-2026-tracker
Osun 2026 election tracker
Osun 2026 Tracker

A single-page, self-contained tracker for the 15 August 2026 Osun State governorship election, covering:

Result Upload — live snapshot of INEC's IReV portal upload progress (polling units uploaded vs. expected, most recent uploads with links to scanned result sheets)
The Field — the full candidate and party ledger for the race
Live site

Once GitHub Pages is enabled for this repo (Settings → Pages → Deploy from branch → main / root), the app is live at:

https://ochijindu.github.io/osun-2026-tracker/
About the data
Upload figures come from IReV's public result API, the same source the official portal (inecelectionresults.ng) uses.
Candidate and party information is compiled from INEC's official candidate list and state election coverage.
Votes are intentionally left as "pending collation." IReV publishes scanned polling-unit result sheets, not tabulated candidate totals — INEC has stated the portal is a viewing tool, not a collation system. Official vote counts are announced separately by the Returning Officer once collation is complete.

This is an independent, unofficial tracker and is not affiliated with or endorsed by INEC.

Updating the data

This is a static HTML file with the data embedded directly in it — there's no backend or build step. To refresh it:

Pull current numbers from IReV's result API
Update the stats, feed, and candidates objects near the bottom of index.html
Commit the change (via the GitHub web UI: open the file, click the pencil/edit icon, paste the update, commit)
Tech

Plain HTML, CSS, and JavaScript. No frameworks, no build tools, no dependencies beyond two Google Fonts loaded via CDN. Works offline aside from font loading.

License

No license specified — all rights reserved by the repository owner.
