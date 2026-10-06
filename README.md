# Trait MMAP

**Trait MMAP (Mapper for Mammals and Parasites)** is a browser-based research tool for rapidly exploring, filtering, spatially selecting, and exporting georeferenced biological data.

Trait MMAP is **upload-first and database-independent**: researchers bring their own CSV, identify coordinate and biological fields, choose traits to explore, and interact with those records on a map without first rebuilding the dataset for a fixed portal schema.

## What Trait MMAP does

**Upload --> configure fields --> filter traits --> explore spatially --> select records --> export**

Trait MMAP currently supports:

- user-uploaded CSV datasets;
- flexible latitude/longitude and metadata field assignment;
- numeric, categorical, and text traits;
- searchable, multi-select categorical filters;
- exact and range-based numeric filtering;
- taxonomic, geographic, temporal, and trait exploration;
- marker clustering and record-density visualization;
- individual, rectangle, and polygon record selection;
- optional terrestrial ecoregion context;
- filtered and selected CSV export;
- filtered and selected GeoJSON export for downstream GIS workflows.

## Scale

Trait MMAP performs filtering and mapping client-side in the browser. During development, the current architecture has successfully operated on a real dataset containing approximately **357,000 records**. This is a demonstrated test scale, not a guaranteed maximum; performance depends on browser, hardware, dataset structure, mapped traits, and the number of displayed records.

## Quick start

1. Open Trait MMAP.
2. Upload a CSV.
3. Assign latitude and longitude.
4. Map useful taxonomic, geographic, temporal, and identifier fields.
5. Choose additional columns as numeric, categorical, or text traits.
6. Build the map.
7. Filter, visualize, and spatially select records.
8. Export the resulting subset as CSV or GeoJSON.

For categorical variables, users can scroll through available values, search within the value list, and select multiple source values simultaneously. Searching within the menu only helps locate choices; checked values determine the actual map filter.

## Why Trait MMAP?

Large biodiversity and specimen datasets may contain coordinates alongside taxonomy, morphology, collection history, host–parasite relationships, and other biological traits. Trait MMAP is intended to reduce the barrier between **obtaining a complex biological table** and **interactively asking spatially explicit questions of it**.

It is an exploratory and subsetting environment rather than a replacement for R, Python, GIS software, or biodiversity databases. Exported subsets can be carried directly into those downstream analytical environments.

## Data and privacy

Core uploaded-data processing occurs in the user's browser. Trait MMAP does not require users to upload their research CSV to a Trait MMAP server. Optional external map/reference services may still receive ordinary web requests needed to provide basemaps or contextual layers.

Researchers remain responsible for appropriate handling of sensitive locality data, restricted specimen information, and source-database licensing or attribution requirements.

## Documentation

- [User guide](docs/USER_GUIDE.md)
- [Preparing data](docs/DATA_FORMAT.md)
- [Validation and performance](docs/VALIDATION.md)

## Project status

Trait MMAP is under active development toward its first public research release. Core upload, filtering, mapping, selection, and export workflows have undergone controlled validation and large-dataset testing.

## Citation

A formal archival citation and DOI will be added with the first versioned public release. Until then, please cite the GitHub repository and version/commit used in your work.

## License

MIT License. See `LICENSE`.
