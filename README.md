# Host Tree Detection and Classification with Google Street View

This repository contains workflows for detecting, classifying, and geolocating urban trees from Google Street View (GSV) imagery.

## Repository Structure

- `/image_downloaders`: scripts for downloading Street View, iNaturalist, and EDDMapS imagery.
- `/tree_detection`: YOLOv5-based tree detection model configuration and training artifacts.
- `/tree_classification`: CNN-based host tree genus classification workflow (preprocess/train/evaluate).
- `/tree_geolocation`: end-to-end geolocation workflow combining detection, classification, and depth estimates.
- `/tree_inventory`: utilities for reconciling model outputs with city inventory data.

## Reproducible Setup

1. Create and activate a Python environment.
2. Install dependencies:
   - `pip install -r requirements.txt`
3. Set `PYTHONPATH` to the repository parent directory:
   - `export PYTHONPATH=$PYTHONPATH:/path/to/parent_directory`
4. Run module workflows using their JSON/YAML config files (see each module README).

## Typical Workflow

1. Download imagery and metadata (`/image_downloaders`).
2. Detect trees in panoramas (`/tree_detection`).
3. Classify detected trees (`/tree_classification`).
4. Geolocate trees from multi-view imagery (`/tree_geolocation`).
5. Join model outputs with city inventories (`/tree_inventory`).

## Citation

If this repository contributes to your work, please cite:

Thomas A. Lake, *Continental-scale computer vision models reveal generalizable patterns and pitfalls for urban tree inventories with street-view images*, ISPRS Open Journal of Photogrammetry and Remote Sensing, https://doi.org/10.1016/j.ophoto.2026.100122.

![Example Tree Detection](https://github.com/ncsu-landscape-dynamics/gsv_host_detector/blob/main/yolov5-prediction-sample-tree.jpg?raw=true)
