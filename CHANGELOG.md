# Changelog

## Unreleased
- Added searchable multi-select categorical filters.
- Removed global all-fields search in favor of field-specific filtering.
- Compiled filter state once per filtering action for substantially improved large-dataset performance.
- Separated complete filtered results from viewport-aware map rendering.
- Preserved strict missing-value behavior and Clear Filters regression fixes.
- Successfully tested the current architecture with a dataset of approximately 357,000 records.
