# Public holiday calendar data

Static JSON files with public holidays, observed days off and make-up working days, one file per
country and year, plus an `index.json` listing every file with its SHA-256 and byte size.

* Index: <https://alice51849.github.io/holiday-calendar-data/index.json>
* Country-year file: `https://alice51849.github.io/holiday-calendar-data/<CC>/<YYYY>.json` (e.g. `TW/2026.json`)
* Schema ids: `offday.holidays-index/v1` (index) and `offday.holidays/v1` (files). Unknown fields must be ignored.
* Every year file carries its `coverage` (verified / rule-derived / uncertain), its `sources` and the
  `attribution` statement its sources require. **The data can be incomplete or wrong; always check the official
  calendar of the country before relying on a date.**

## Licences

The compilation is licensed **CC BY 4.0** (`LICENSES/CC-BY-4.0.txt`). Source-specific licence texts are in
`LICENSES/` (OGDL-TW-1.0, Open Government Licence v3.0, Licence Ouverte / Open Licence 2.0, Public Data
License 1.0, KOGL Type 1, Singapore Open Data Licence 1.0, MIT for python-holidays rules) and `LICENSES/NOTICES.txt`
explains which applies where. Attribution statements are repeated verbatim in each year file.

## Publishing

Files are produced and verified by a generator (`generate.py --check`) and pushed by a script; there are no
workflows or secrets in this repository. Contact: hourstag.app@gmail.com
