# PCB-MDD-Curated Dataset
PCB Manufacturing Defect Detection - Curated Dataset

## Overview
A curated and enhanced dataset for PCB defect detection with 6 common manufacturing defects. This dataset is cleaned, corrected, and optimized for machine learning research.

## Dataset Statistics
- **Total Images**: 8,240
- **Classes**: 6 defect types
- **Training set**: 6,370 images
- **Validation set**: 802 images
- **Test set**: 1,068 images
- **Image resolution**: 640×640 pixels
- **Format**: YOLO format (compatible with Ultralytics YOLO)

## Defect Classes
1. `0` - Missing Hole
2. `1` - Depaneling Damage
3. `2` - Open Circuit
4. `3` - Short
5. `4` - Spur
6. `5` - Spurious Copper

## Dataset Structure

PCB-MDD-Curated/
├── train/
│ ├── images/ # Training images
│ └── labels/ # YOLO format annotations
├── val/
│ ├── images/ # Validation images
│ └── labels/ # YOLO format annotations
└── test/
├── images/ # Test images
└── labels/ # YOLO format annotations

## Citation
If you use this dataset in your research, please cite:

```bibtex
@dataset{pcb_mdd_curated_2026,
  title = {PCB-MDD-Curated: A Curated PCB Manufacturing Defect Detection Dataset},
  author = {Md Sohel Rana},
  year = {2026},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.18318110},
  url = {https://doi.org/10.5281/zenodo.18318110}
}
```
Usage with YOLO
Clone this repository

Update the dataset path in pcb-mdd-curated.yaml

Train your model:
```
from ultralytics import YOLO
model = YOLO('yolov8n.pt')
model.train(data='pcb-mdd-curated.yaml', epochs=100)
```
License
This dataset is released under the MIT License. See LICENSE file for details.

Contact
For questions or issues, please open an issue on GitHub.
