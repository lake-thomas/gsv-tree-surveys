# Tree Geolocation

The `tree_geolocation` module provides scripts that combine tree detection (YOLOv5), classification (CNN), and depth estimation to geolocate street trees from Google Street View imagery.

## Files

- **geolocate.py**: Python script applying the tree detection, image classification, and depth estimation models to geolocate trees.
- **geolocation_config.json**: Config file for geolocate.py to specify paths for models, images to use for geolocation, and tree genera to identify.
- **geoutilities.py**: Python function library to load models, process imagery, apply model predictions, and geolocate trees.
- **/jupyter_notebooks**: Notebooks to experiment with tree geolocation workflows.

## Usage

1. Export Python path to the repository parent directory:
   - `export PYTHONPATH=$PYTHONPATH:/path/to/parent/directory`

2. Activate your environment with required dependencies.

3. Update `geolocation_config.json` with model paths, image paths, and output options.

4. Run geolocation:
   - `python -m tree_geolocation.geolocate --config "/path/to/geolocation_config.json"`
