# AI-Assisted Pneumonia Classification from Lung Ultrasound

An educational computer-vision project exploring whether a pretrained model can classify lung-ultrasound images using pneumonia and normal labels.

## Project status
Planning and environment setup. Dataset permissions and access must be verified before any data is downloaded or used.

## Intended approach
- Start with a pretrained image-classification model.
- Split data by video before extracting frames.
- Evaluate on held-out videos using precision, recall, F1-score, and balanced accuracy.
- Build a small demonstration only after evaluating the model.

## Important limitations
This is a learning project, not a clinically validated medical device. Its outputs must not be used to diagnose or guide treatment. Dataset videos are not included in this repository.

## Repository contents
- `PROJECT_PLAN.md` — project scope and workflow.
- `DATASET.md` — dataset description and permission checks.
- `EXPERIMENT_LOG.md` — experiment records.
- `requirements.txt` — project dependencies.
- `notebooks/` — Colab notebooks.
- `src/` — planned source code.
