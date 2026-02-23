# Tree Geolocation

The 'tree_geolocation' module provides Python scripts to apply tree object detection (YOLOv5) and image classification (CNN), and depth estimate (ZoeDepth) models to geolocate street trees from Google Street View imagery.

## Files

- **geolocate.py**: Python script applying the tree detection, image classification, and depth estimation models to geolocate trees.
- **geolocation_config.json**: Config file for geolocate.py to specify paths for models, images to use for geolocation, and tree genera to identify.
- **geoutilities.py**: Python function library to load models, process imagery, apply model predictions, and geolocate trees.
- **/jupyter_notebooks**: Notebooks to experiment with tree geolocation workflows.

## Usage

1. Export Python path to the parent directory of `tree_geolocation`:
   `export PYTHONPATH=$PYTHONPATH:/path/to/parent/directory`
2. Load a conda environment with PyTorch:
   `source activate my_env`
3. Inspect `geolocation_config.json` to specify model, image, and output paths.
4. Run geolocation:
   `python -m tree_geolocation.geolocate --config "/path/to/geolocation_config.json"`
