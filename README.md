# penseur-map-levels

Map data for Penseur's map, cut into levels of detail that a Penseur box can download.

Each release holds the level files, split into parts where a file is over GitHub's per-file limit, and a
`levels.json` naming every level's zoom range, parts, sizes and SHA-256. A box downloads the parts, joins them and
checks every hash before it uses a level.

The files are made by a workflow in `penseurai/penseur-os` (`.github/workflows/map-levels.yml`). Nothing in this
repository is edited by hand.

## Data and licence

The vector tiles are cut from [OpenFreeMap](https://openfreemap.org)'s planet build, which uses the
[OpenMapTiles](https://openmaptiles.org) schema.

- Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), available under the
  [Open Database Licence (ODbL)](https://opendatacommons.org/licenses/odbl/).
- Tile schema © [OpenMapTiles](https://openmaptiles.org).

Any map drawn from these files must show this attribution. Penseur's map keeps it visible.
