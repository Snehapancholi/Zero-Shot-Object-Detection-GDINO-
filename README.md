# Zero-Shot Object Detection using Grounding DINO (GDINO)

## Overview
Traditional object detection models such as YOLO or Faster R-CNN are limited to a fixed set of predefined object classes.
This project demonstrates **zero-shot object detection** using **Grounding DINO (GDINO)**, where objects are detected
based solely on **natural language prompts**, without requiring any task-specific training.

The project explores how prompt formulation, confidence thresholds, and model backbone choice affect detection quality.

---

## Model Details
- **Model:** Grounding DINO
- **Backbone:** Swin-B (Swin Transformer – Base)
- **Framework:** HuggingFace Transformers
- **Approach:** Prompt-based zero-shot object detection

---

## Key Features
- Detect objects using natural language prompts
- No training or fine-tuning required
- Supports detection of unseen / open-set objects
- Visualization of bounding boxes with confidence scores
- Analysis of successful and failed detections

---

## Project Structure
Zero-Shot-Object-Detection-GDINO/
│
├── README.md
├── requirements.txt
├── notebooks/
│   └── gdino_zero_shot_detection.ipynb
│
├── images/
│   ├── input/
│   └── output/
│
└── src/ (optional)


---

## Dataset
- Custom images (desk setups, indoor scenes)
- Open-source images from Unsplash / Pexels
- Optional evaluation on COCO or Open Images subsets

No labeled training data is required due to the zero-shot nature of the model.

---
## Installation
Install dependencies using:
```bash
pip install -r requirements.txt
texts = ["lamp", "a desk lamp", "table lamp"]
threshold = 0.3
