# [WasteVision - Workshop WACV 2026] SortWaste: A Densely Annotated Dataset for Object Detection in Industrial Waste Sorting

This repository provides resources associated with the paper  
**“SortWaste: A Densely Annotated Dataset for Object Detection in Industrial Waste Sorting”**, presented at the *WACV Workshop*.

SortWaste is a **real-world industrial object detection dataset**, collected on a municipal solid waste (MSW) sorting line. It focuses on highly challenging visual conditions, including **dense clutter, object overlap, deformation, and contamination**, which are typically underrepresented in existing waste datasets.

## Dataset Overview

The SortWaste dataset consists of top-down images of waste items on a conveyor belt, densely annotated with bounding boxes. The scenes reflect real industrial sorting conditions and are designed to evaluate object detection models under high visual complexity.

The following figure shows **annotated samples from the dataset**, illustrating object density, clutter, and the diversity of materials.  
**Note:** this image provides an overview of the annotated dataset and **does not depict the data collection setup**.

![images](images/teaser(2).png)

## Annotated Classes

SortWaste includes **8 waste material classes**, annotated with bounding boxes:

- **HDPE** – Opaque rigid plastics (e.g., detergent bottles, yogurt containers)
- **PET** – Transparent or green rigid plastics (e.g., beverage bottles)
- **PET Oil** – PET containers used for edible oils (treated as a PET subcategory)
- **Mixed Soft Plastic** – Flexible plastics (e.g., bags, snack wrappers)
- **Mixed Rigid Plastic** – Rigid plastics not classified as HDPE
- **ECAL** – Multi-layer liquid food packaging (e.g., milk and juice cartons)
- **Cardboard** – Corrugated or flat cardboard packaging
- **Metal** – Metallic packaging such as cans and tins

Representative examples of each class are shown below:

![images](images/classes.png)

## Dataset Characteristics

- 📦 **5,261 annotated images**
- 🔲 **87,000+ bounding boxes**
- 🏭 Captured in a real industrial sorting environment
- 👁️ High object density and frequent occlusions
- 🔄 Large variability in object scale, shape, and condition

## Purpose

SortWaste is intended as a **realistic benchmark** for:
- Object detection in industrial waste-sorting environments
- Robustness analysis under heavy clutter and overlap
- Research on automated waste sorting systems

In addition to the dataset, the paper introduces **ClutterScore**, a metric designed to quantify scene visual complexity and analyze its impact on detection performance.

## Citation

If you use this dataset or related resources, please cite:

```bibtex
@misc{inácio2026sortwastedenselyannotateddataset,
  title        = {SortWaste: A Densely Annotated Dataset for Object Detection in Industrial Waste Sorting},
  author       = {Sara Inácio and Hugo Proença and João C. Neves},
  year         = {2026},
  eprint       = {2601.02299},
  archivePrefix= {arXiv},
  primaryClass = {cs.CV},
  url          = {https://arxiv.org/abs/2601.02299},
} 
