# Optimizing Wind Turbine Surface Defect Detection: A Rotated Bounding Box Approach
This repository contains rotated bounding box annotations for DTU-Drone inspection images and Blade30 datasets.

## Introduction
Detecting surface defects on Wind Turbine Blades (WTBs) from remotely sensed images is a crucial step toward automated visual inspection. Typical object detection algorithms use standard bounding boxes to locate defects on WTBs. However, Oriented Bounding Boxes (OBBs) have been shown in cases of satellite imagery, to provide more precise localization of object regions and actual orientation. Existing WTB datasets do not depict defects using OBBs and this causes the lack of useful orientational information. In this paper, we consider OBBs for WTB surface defect detection through two publicly available datasets, introducing new annotations to the community. Baselines were constructed on state-of-the-art rotated object detectors, demonstrating considerable promise and known gaps that can be addressed in the future. We present a comprehensive analysis of their performances including ablation study and discussions on the importance of angular disparity between OBBs.

Standard Bounding Box vs. Oriented Bounding Box:

<img src="![bb_comparison](https://github.com/imadgohar/Rotated_BB_Annotations/assets/45845910/9bc8363d-d253-4c64-8f52-9dab49be37c9" alt="bb_comparison" width="600">

## Advantages Over standard BBox
- OBB localization is more tighter than standard BB
- Help in reducing overlapping areas
- Better for dense objects

## Visual Results
Comapring Jensen-Shannon Distribution (JSD) - symmetric, Gaussian Wasserstein Distance (GWD), RIoU and Hybrid Loss function.
<img src="![RFcos_Test_set_results_comparison_cropped (1)](https://github.com/imadgohar/Rotated_BB_Annotations/assets/45845910/b3505027-f744-42b3-9f37-520d72b6ea9d" alt="bb_comparison" width="600">


# Project Poster

<img src="" alt="bb_comparison" width="600">

## Datasets
DTU-Drone Inspection images and Blade30

## Citation
~~~bibtex
@inproceedings{gohar2024optimizing,
  title={Optimizing Wind Turbine Surface Defect Detection: A Rotated Bounding Box Approach},
  author={Gohar, Imad and Halimi, Abderrahim and Kean, Yew Weng and See, John},
  booktitle={32nd European conference on signal processing 2024},
  year={2024}
}
