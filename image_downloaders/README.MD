# Image Downloaders

Utilities for downloading imagery and metadata used throughout the project.

## Files

- `get_panos_and_metadata_async_csv.py`: download Google Street View panoramas and metadata from CSV input points.
- `downloader_config_csv.json`: example configuration for the GSV downloader.
- `tiny_25m_near_samples.csv`: sample point file for testing downloads.
- `osmnx_functions.py`: helper functions for OpenStreetMap road-network processing.
- `r_scripts/inat_img_dler.R`: download iNaturalist images.
- `r_scripts/eddmaps_img_dler.R`: download EDDMapS images.

## Usage (GSV Downloader)

1. Set `PYTHONPATH` to the repository parent directory.
2. Activate your environment with required dependencies.
3. Update `downloader_config_csv.json` with API key path, input points, and output locations.
4. Run:
   - `python -m image_downloaders.get_panos_and_metadata_async_csv --config "/path/to/downloader_config_csv.json"`
