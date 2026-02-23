# Host Tree Detection and Classification with Google Street View

This repository contains code for detecting, classifying, and geolocating trees using Google Street View imagery.

## Citation

If you use this repository, please cite:

Lake et al., 2026. Continental-scale computer vision models reveal generalizable patterns and pitfalls for urban tree inventories with street-view images, *ISPRS Open Journal of Photogrammetry and Remote Sensing*, 10.1016/j.ophoto.2026.100122.

## Reproducible Workflow

1. Install dependencies from `/requirements.txt`.
2. Download imagery with `/image_downloaders`.
3. Detect trees in panoramic imagery with `/tree_detection`.
4. Classify detected trees with `/tree_classification`.
5. Geolocate trees with `/tree_geolocation`.
6. Compare with city inventory records in `/tree_inventory`.

## Repository Structure

- `/image_downloaders`: Download iNaturalist and Google Street View images.
- `/tree_detection`: YOLOv5-based object detection resources for tree detection.
- `/tree_classification`: CNN training and evaluation for host tree classification.
- `/tree_geolocation`: Integrated detection/classification/depth workflow for geolocating trees.
- `/tree_inventory`: Scripts for matching model outputs with city inventory records.

![Example Tree Detection](https://github.com/ncsu-landscape-dynamics/gsv_host_detector/blob/main/yolov5-prediction-sample-tree.jpg?raw=true)
