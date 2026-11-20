## Science API endpoints, snapshot 15 Nov 2026

- 384,890 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 6,223 services · 248 country codes · 206,647 keyless JSON rows

### Download

- `Science_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 384,890 rows, 9.2 MB gzipped (94.4 MB as CSV), SHA-256 `b10132b6fb35efc891dca8444da7947399e3c55de23cfbd46b3a79396a21a0e6`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Science_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Science_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 2,870 · Wrap one sun-times URL as a get_sun_times tool: pass a latitude and longitude, return sunrise, sunset and day length; add space-weather and GBIF lookups as separate tools with a timeout.
- 📱 App features: 12,574 · Show the geology under a place on a map: load a bedrock or surficial layer for one area and return unit name, age and rock type for a clicked point.
- 🧠 Grounding and data pipelines: 54,693 · Load research-project lists, R&D statistics and biodiversity dataset searches on a schedule into your own store, so answers about who studies what cite a dated source.
- 🧪 Evals and testing: 384,890 · Run your science tool against a fixed set of URLs across formats (XML feature requests, KML, JSON and CSV); check that times, coordinates and attribute values parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 478 rows with a private or local address.
- Left out: 15 rows with an email-like address.
- Left out: 257 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 4 layers marked editable in the title (they can hold entries that people added).
- Left out: 34 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 86 rows that passed a data call only from a network location in India.
- Left out: 39 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 3,348 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 133 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 6,521 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 5,730 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 109,513 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 3,814 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 86 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 206,647 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 152 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 61 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 100 of these URLs are also in 10k-earthquake-apis-for-agents.
- Overlap: 79 of these URLs are also in 5.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Science API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
