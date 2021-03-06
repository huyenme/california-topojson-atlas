# california-topojson-atlas

Simple maps of California's 58 counties

### Usage

* In the browser [using d3 and SVG](https://observablehq.com/@datadesk/base-maps-for-all-58-california-counties)

### Data dictionary

The [`output`](output/) directory contains a topojson file for each of the state's 58 counties. The files are named using the county's [FIPS code](https://en.wikipedia.org/wiki/Federal_Information_Processing_Standards) and contain three layers:

* `county`: The outline of the county
* `roads`: Major roads in the county
* `places`: All [Census-defined places](https://en.wikipedia.org/wiki/Census-designated_place) in the county, along with their population.

### Sources

The following data sources are stored in the [`input`](input/) directory:

* County shapes from the U.S. Census Bureau
* Roads from [Natural Earth](https://www.naturalearthdata.com/downloads/10m-cultural-vectors/roads/)
* Places from the U.S. Census Bureau via [Census Reporter](https://censusreporter.org/)

### Installation

The [`mapshaper`](https://github.com/mbloch/mapshaper) utility is required to run this repository. Install it.

Clear out all the built files.

```bash
make clean
```

Run the `make` command that regenerates all the files in the output folder.

```bash
make
```
