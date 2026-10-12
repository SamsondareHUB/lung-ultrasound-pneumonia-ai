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
The COVIDx-US repository is licensed under GPL-3.0, but the underlying
videos come from multiple sources with differing terms. The repository
identifies some sources with Creative Commons licenses and others without
license information. Verify permission from each source for the intended
research use before downloading, using, or sharing any video.

Do not redistribute videos or derived data unless the applicable terms allow it.

## Limitations
The dataset is small and combines multiple sources. Results may not generalize
to other hospitals, devices, or patient populations. This is an educational
prototype, not a clinically validated diagnostic tool.
