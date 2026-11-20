## Ocean and marine API endpoints, snapshot 15 Nov 2026

- 86,107 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 2,241 services · 129 country codes · 68,292 keyless JSON rows

### Download

- `Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 86,107 rows, 3.1 MB gzipped (27.1 MB as CSV), SHA-256 `696976e1bb225d1638e671fd4cccdd8906bd81528a4d3227f8aedc594f1ae17c`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 1,409 · Wrap one station URL as a get_sea_level or get_sea_temperature tool: pass the station code, return the latest value, its unit and time, with a timeout. Dataset records and map layers in this list need a query of their own.
- 📱 App features: 8,394 · Draw protected areas, sea level rise zones or reef layers on a coastal map: each layer query returns features with names and classes you can show on a card.
- 🧠 Grounding and data pipelines: 65,097 · Read each ERDDAP description for its variables and time range, then load the series from tabledap or griddap on a schedule into your own store, so answers about sea conditions cite a dated source.
- 🧪 Evals and testing: 86,107 · Run your ocean tool against a fixed set of URLs across formats; check that time, value, unit and position parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 130 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 415 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 3 layers marked editable in the title (they can hold entries that people added).
- Left out: 14 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 99 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 9 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 22 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Overlap: 5,687 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 1,384 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 86,107 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 805 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 1,115 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 1,157 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 82 of these URLs are also in 290k-statistics-apis-for-agents.
- Overlap: 2,484 of these URLs are also in 24k-maritime-apis-for-agents.
- Overlap: 4,201 of these URLs are also in 170k-environment-apis-for-agents.
- Overlap: 25 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 1,729 of these URLs are also in 380k-maps-gis-apis-for-agents.
- Overlap: 68,292 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 6 of these URLs are also in 96k-health-apis-for-agents.
- Overlap: 3,814 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 549 of these URLs are also in 53k-hazards-apis-for-agents.
- Overlap: 6 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 66 of these URLs are also in 72k-energy-apis-for-agents.
- Overlap: 31 of these URLs are also in 25k-aviation-apis-for-agents.
- Overlap: 970 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 5 of these URLs are also in 12k-parking-apis-for-agents.
- Overlap: 90 of these URLs are also in 10k-earthquake-apis-for-agents.
- Overlap: 64 of these URLs are also in 5.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Ocean and marine API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
