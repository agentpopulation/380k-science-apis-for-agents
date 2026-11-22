# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 384,890 endpoints from 6,223 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 383,715 endpoints from 5,924 services, 1,175 fewer endpoints than first published under this snapshot (384,890 from 6,223 services), tested 10–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Science_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 380k-science-apis-for-agents (was science-api-endpoints).
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
