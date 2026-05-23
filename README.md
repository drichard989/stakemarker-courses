# StakeMarker Courses

A derived golf-course database used by the [StakeMarker](https://stakemarker.com) app.

This dataset is **derived** from [OpenGolfAPI](https://opengolfapi.org/) — it is a
filtered, field-reduced subset containing only:

- Course name and location (city, state)
- Per-hole par values
- Per-hole stroke (handicap) index

Coordinates, contact details, architect, yardage, and other fields from the
source dataset have been removed.

## Files

| File | Description |
|------|-------------|
| `courses.json` | Array of course records: `{ id, name, city, state, source, pars[18], hcps[18] }` |
| `courses-meta.json` | `{ version, count }` — version is the UTC sync date |

These files are synced automatically from the source dataset; do not edit by hand.

## License & Attribution

This is a derivative database made available under the
**[Open Database License (ODbL) v1.0](https://opendatacommons.org/licenses/odbl/1-0/)**,
the same license as the source.

> Contains information from OpenGolfAPI, which is made available under the
> Open Database License (ODbL).

See [`LICENSE.txt`](LICENSE.txt) for the full license text.
