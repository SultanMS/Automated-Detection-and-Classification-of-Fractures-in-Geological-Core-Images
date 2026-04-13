# Automated Detection and Classification of Fractures in Geological Core Images

This repository provides the source code for automated detection and classification of fractures in slabbed geological core images using:

- Mask R-CNN (instance segmentation)
- YOLOv8-seg (one-stage instance segmentation)
- U-Net (semantic segmentation)

The models distinguish between:
- Natural fractures
- Induced fractures

## Dataset Format

The dataset is expected in **LabelMe format**:

- Each image has a corresponding `.json` file
- JSON contains:
  - `"imagePath"` → image filename
  - `"shapes"` → list of annotated polygons

### Supported labels:
- `"natural fracture"`
- `"induced fracture"`
