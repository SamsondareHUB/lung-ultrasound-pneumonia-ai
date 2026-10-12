# Dataset Notes

## Dataset name
COVIDx-US

## Dataset repository
https://github.com/nrc-cnrc/COVID-US

## Dataset description
The repository reports 242 lung-ultrasound videos in four categories:
COVID-19, Pneumonia, Normal, and Other. The reported video counts include
49 Pneumonia videos and 28 Normal videos.

The repository does not host the underlying ultrasound videos; it describes
data collected from multiple external sources.

## Proposed task
If data access and permitted use are confirmed, investigate a binary
classification experiment using the repository's Pneumonia and Normal labels.
Do not include COVID-19 or Other cases in this initial task.

## Split plan
- Split by video, never by extracted frame.
- Keep every frame from one video in a single split.
- Document the exact video IDs and class counts for each split.
- Do not begin model training until the permitted data sources and labels
  have been verified.

## Usage and permissions

The COVID-US repository is an open-source project under AGPL-3.0. This does not
automatically grant permission to use every underlying video.

The COVID-US README lists these source terms:
- The POCUS Atlas: CC BY-NC 4.0.
- LITFL: CC BY-NC-SA 4.0.
- Radiopaedia: CC BY-NC-SA 3.0.
- ButterflyNetwork, GrepMed, CoreUltrasound, and Clarius: no data-use license
  information is listed in the COVID-US README.

For the first experiment, exclude sources without explicit data-use terms.
Before using any other video, verify its source page, attribution requirements,
license conditions, and whether the planned research and any sharing are allowed.
Do not upload source videos, extracted frames, or derived data to this repository.

This project is educational and non-clinical. Ask the relevant rights holder or
institution if the intended use or license conditions are unclear.

## Limitations
The dataset is small and combines multiple sources. Results may not generalize
to other hospitals, devices, or patient populations. This is an educational
prototype, not a clinically validated diagnostic tool.
