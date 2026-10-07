# License Plate Detection

## Team Members

* Chris Roy
* Njeh ABABIO
* Unnati Shakya
* Edwin Marquez

---

## Project Tier

**Tier 1 — Core**

This project uses a single computer vision model to perform one focused task: detecting license plates in vehicle images.

---

## Problem Statement

Identifying license plates across large numbers of vehicle images can be time-consuming and inconsistent when performed manually. A computer vision system that automatically locates license plates could make vehicle-image processing faster, more consistent, and easier to scale.

---

## Solution Overview

We will build a license plate detection application using a YOLO object detection model. Given an image containing one or more vehicles, the model will identify the locations of visible license plates and display them using bounding boxes.

### Workflow

**Vehicle Image → YOLO Detection Model → License Plate Bounding Boxes**

The project will focus on detecting the location of license plates and will not attempt to read the characters on the plates.

---

## Technical Approach

### Computer Vision Technique

**Object Detection**

### Model

**YOLO (You Only Look Once)**

### Framework

**Ultralytics YOLO with PyTorch**

### Model Strategy

We plan to begin with a pretrained YOLO model and fine-tune it using a labeled license plate dataset.

### Why This Approach?

YOLO is designed for fast object detection and can identify objects using bounding boxes. This makes it a practical fit for a focused Tier 1 project while leaving room for future improvements if needed.

---

## Data Plan

### Data Source

**WIP — Public license plate dataset to be selected by the group**

### Approximate Dataset Size

**WIP**

### Images

Vehicle images containing visible license plates.

### Labels

License plates will be labeled using bounding boxes indicating their locations within the images.

### Data Preparation

We will review the dataset for incorrect or missing annotations. The available data will then be divided into training, validation, and test sets.

### Dataset Link

**WIP — Add public dataset URL after the group selects the dataset.**

---

## Success Metrics

### Primary Metric — mAP@50

**Target: ≥ 0.70**

The primary metric will measure how accurately the model detects license plates using predicted bounding boxes.

### Secondary Metric — Precision

**Target: ≥ 0.80**

Precision will measure how often the model's detected objects are actually license plates.

### Overall Success

The project will be considered successful if the model reliably detects license plates across a variety of vehicle images while maintaining a relatively low number of false detections.

---

## Milestone Plan

> **WIP — Final schedule will be confirmed by the group.**

| Phase              | Timeline  | Goal                                                                              |
| ------------------ | --------- | --------------------------------------------------------------------------------- |
| Blueprint          | Week 5    | Finalize project scope, dataset plan, and technical approach                      |
| First Working Demo | Week 6    | Run a pretrained YOLO model on sample images and produce license plate detections |
| Make It Yours      | Weeks 7–8 | Fine-tune the model and build the license plate detection workflow                |
| Improve & Measure  | Week 9    | Evaluate performance, tune the model, and document results                        |
| Package & Present  | Week 10   | Finalize the notebook, README, demo, and presentation                             |

---

## Risks and Plan B

### Risk 1 — Dataset Quality

The selected dataset may contain inconsistent, missing, or difficult-to-detect license plate annotations
