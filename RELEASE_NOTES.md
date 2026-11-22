## Science API endpoints, snapshot 15 Nov 2026

- 383,715 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 5,924 services · 248 country codes · 205,472 keyless JSON rows

### Download

- `Science_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 383,715 rows, 9.1 MB gzipped (93.2 MB as CSV), SHA-256 `18587254f15928fa85e15995f746d5788e14bde5b18b5ec93ad1b64f8a3f526a`
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
- 📱 App features: 11,879 · Show the geology under a place on a map: load a bedrock or surficial layer for one area and return unit name, age and rock type for a clicked point.
- 🧠 Grounding and data pipelines: 52,143 · Load research-project lists, R&D statistics and biodiversity dataset searches on a schedule into your own store, so answers about who studies what cite a dated source.
- 🧪 Evals and testing: 383,715 · Run your science tool against a fixed set of URLs across formats (XML feature requests, KML, JSON and CSV); check that times, coordinates and attribute values parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 384,890 endpoints from 6,223 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 383,715 endpoints from 5,924 services, 1,175 fewer endpoints than first published under this snapshot (384,890 from 6,223 services), tested 10–15 Nov 2026 (IST).
- Left out: 478 rows with a private or local address.
- Left out: 15 rows with an email-like address.
- Left out: 257 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 15 ArcGIS proxy layers (utility.arcgis.com/usrsvcs and portal /sharing/servers/ addresses) that can call a service with a stored login.
- Left out: 4 layers marked editable in the title (they can hold entries that people added).
- Left out: 34 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 86 rows that passed a data call only from a network location in India.
- Left out: 45 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 6 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 8 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 193 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 21 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 924 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 2 rows that repeat an address already in the pack.
- Overlap: 3,348 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 134 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 6,523 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 5,730 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 109,513 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 4 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 3,814 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 8 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 86 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 37 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 205,459 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 1 of these URLs is also in 40k-hazards-apis-for-agents.
- Overlap: 152 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 5 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 61 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 101 of these URLs are also in 7.8k-earthquake-apis-for-agents.
- Overlap: 79 of these URLs are also in 4.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Science API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
