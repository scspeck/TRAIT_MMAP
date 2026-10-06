# Preparing data for Trait MMAP

Trait MMAP accepts CSV files with one header row and one record per subsequent row.

## Required for mapping
- latitude in decimal degrees (-90 to 90);
- longitude in decimal degrees (-180 to 180).

Rows without valid coordinates may remain in the source CSV but cannot be mapped.

## Useful fields
Scientific name, family, genus, species, country, state/province, county, locality, collection date/year, stable specimen identifier or GUID, sex, life stage, measurements, parasite identity, and parasite counts or richness.

## Trait types
**Categorical:** discrete source values such as genus, sex, state, life stage, or parasite family. Values remain distinct; for example `F`, `Female`, and `female` can all be selected together without altering the original data.

**Numeric:** measurements or counts. Numeric filters can use exact, minimum, and maximum criteria.

**Text:** free-form values such as remarks or locality descriptions.

Trait MMAP preserves source values for export.
