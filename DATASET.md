# Dataset Notes

## Dataset name
Lung Ultrasound Imaging Dataset for Accurate Detection and Localization of LUS Vertical Artifacts (LUS-BALD), Version 2

## Source
https://data.mendeley.com/datasets/h923m366sf/2

## Dataset summary
The dataset contains 401 high-resolution lung-ultrasound images from 255 patients at Mulago and Kiruddu National Referral Hospitals in Uganda. Polygon annotations identify lung-ultrasound vertical artifacts.

## Intended task
Detect and localize annotated vertical artifacts commonly referred to as B-lines. This project does not classify or diagnose pneumonia.

## License and attribution
The dataset is listed under Creative Commons Attribution 4.0 International (CC BY 4.0). Follow the license requirements, cite the dataset DOI (10.17632/h923m366sf.2), and credit the dataset contributors when using or sharing permitted material.

## Data handling
- Keep downloaded images outside this GitHub repository.
- Inspect the annotation format before selecting a model.
- If patient identifiers are available, split by patient so images from one patient do not appear across multiple splits.
- Do not upload images, annotations, or derived data unless permitted by the dataset terms.

## Limitations
Vertical artifacts are ultrasound findings, not a diagnosis of pneumonia. They can be associated with multiple pulmonary conditions. This educational prototype is not clinically validated and must not guide diagnosis or treatment.
