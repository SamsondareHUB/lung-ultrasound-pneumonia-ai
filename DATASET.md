# Dataset Notes

## Dataset name
COVIDx-US

## Source
https://github.com/nrc-cnrc/COVID-US

## Intended task
Binary classification using video-level labels:
- Pneumonia
- Normal

COVID-19 and other lung-condition cases are excluded from this first experiment.

## Label definitions
Use the labels provided in the official COVIDx-US metadata. Do not create labels from individual frames or infer diagnoses from image appearance.

## Data and split plan
- Keep dataset files outside this GitHub repository.
- Split by video before extracting frames.
- Keep all frames from one video in only one split.
- Record video counts per class for training, validation, and test sets before training.
- Do not use COVID-19 or "Other" cases in the initial binary experiment.

## Usage and license
The COVIDx-US repository is distributed under AGPL-3.0, but the underlying data come from multiple sources with different or unclear permissions. Review the dataset README and the terms for each source before downloading, using, or sharing data. Do not redistribute images or videos unless their terms permit it.

## Known limitations
The dataset is small and assembled from multiple sources. Results may not generalize to other hospitals, devices, or patient populations. This is an educational prototype and is not for clinical diagnosis.
