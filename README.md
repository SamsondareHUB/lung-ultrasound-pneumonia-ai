# LUS Vertical Artifact Segmentation with YOLO11

This project trains and evaluates a YOLO11 instance-segmentation baseline for detecting and localizing vertical artifacts in lung ultrasound (LUS) images.

## Dataset

The project uses the publicly available **LUS-BALD** dataset:

- **Dataset:** Lung Ultrasound Imaging Dataset for Accurate Detection and Localization of LUS Vertical Artifacts  
- **Paper:** https://doi.org/10.1038/s41597-025-05854-4  
- **Data repository:** https://data.mendeley.com/datasets/h923m366sf  

LUS-BALD contains 401 lung ultrasound images split at the patient level into training, validation, and test sets. Polygon annotations are provided for the training and validation sets; the 70 test images are intended for blind evaluation and do not include labels in the public release. [265]

## Model

- **Task:** Instance segmentation  
- **Model:** YOLO11n-seg  
- **Input size:** 640 × 640  
- **Training epochs:** 50  
- **Class:** `vertical_artifact`  

## Results

The model was trained on 256 labeled training images and evaluated on 75 labeled validation images.

| Metric | Value |
|---|---:|
| Mask precision | 0.796 |
| Mask recall | 0.848 |
| Mask mAP50 | 0.876 |
| Mask mAP50–95 | 0.443 |

These are validation results. The test split was used only for visual inspection of predictions because its annotations are not publicly available.

## How to run

Install the required package:

```bash
pip install ultralytics
```

Train the model:

```python
from ultralytics import YOLO

model = YOLO("yolo11n-seg.pt")

model.train(
    data="data.yaml",
    epochs=50,
    imgsz=640,
    batch=8,
)
```

Run predictions:

```python
from ultralytics import YOLO

model = YOLO("path/to/best.pt")

model.predict(
    source="path/to/images",
    imgsz=640,
    conf=0.25,
    save=True,
)
```

## Files

- `lus_bald_baseline.ipynb` — Colab notebook containing the training and prediction workflow.
- `data.yaml` — Dataset configuration used by Ultralytics.
- `lus_bald_yolo11n_seg_best.pt` — Trained YOLO11 segmentation checkpoint.
- `lus_bald_yolo11n_seg_best.onnx` — ONNX export for portable inference.

## Notes

- This repository does **not** redistribute the LUS-BALD dataset.
- The model is a research baseline and is not intended for clinical diagnosis or medical decision-making.
