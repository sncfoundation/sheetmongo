<p align="center">
  <img src="https://sncfoundation.github.io/logos/sheetmongo.svg" width="96" alt="SheetMongo logo">
</p>

<h1 align="center">SheetMongo</h1>

<p align="center"><b>A document store — each row is a JSON document.</b><br>
A <a href="https://sncfoundation.github.io">Sheet-Native Computing Foundation</a> project · the spreadsheet-native <b>MongoDB</b></p>

---

**Status:** 📝 Unsaved Draft (design). Data & Storage TAG.

## The mapping

- **collection** = a tab; **document** = a row with a JSON blob (or `_id` + JSON columns).
- **find/aggregate** = `QUERY()` + Apps Script JSON parsing; **index** = a helper/sorted column; **shard** = multiple tabs/sheets.

## Honest limit

**50k characters per document** (the cell cap); no true secondary indexes (scan or helper column); aggregation is slow.

## Connect with real clients

Paired with [SheetWire](https://github.com/sncfoundation/sheetwire), real MongoDB clients can connect to a Google Sheet over the native wire protocol.

- 🗺️ [SNCF Landscape](https://sncfoundation.github.io/landscape.html) · 🧩 [Projects](https://sncfoundation.github.io/projects.html) · 🎓 [Certification](https://sncfoundation.github.io/certification.html)

---

<sub>Apache-2.0. Do not run production data on a spreadsheet. If you do, please film the query plan.</sub>
