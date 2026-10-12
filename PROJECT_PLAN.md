# Project Plan

## Project title
B-Line Detection in Lung Ultrasound Images Using Deep Learning

## Project goal
Build an educational computer-vision prototype that detects and localizes B-line artifacts in lung-ultrasound images using annotated data.

## Project question
Can a pretrained object-detection model identify annotated B-line regions in held-out lung-ultrasound images?

## Proposed dataset
LUS-BALD: a dataset of lung-ultrasound images with polygon annotations of vertical artifacts. Verify the dataset files, patient identifiers, and license conditions before using the data.

## Scope
- Focus on detecting/localizing B-line artifacts, not diagnosing pneumonia.
- Start with a pretrained object-detection model.
- Split by patient before training if patient identifiers are available.
- Do not upload dataset images or derived images to this repository.
- Treat this as an educational prototype, not a clinical tool.

## Initial workflow
1. Inspect the dataset documentation, files, annotations, and usage terms.
2. Confirm how polygon annotations should be converted for the selected model.
3. Create patient-level train, validation, and test splits if patient IDs are available.
4. Train a pretrained baseline model.
5. Evaluate localization on held-out patients using suitable detection metrics.
6. Record experiments and limitations.

## Evaluation
Choose detection metrics after inspecting the annotation format. Report the patient-level split method, class definitions, and any limitations.

## Safety and limitations
This project does not diagnose pneumonia or any other disease. B-lines can occur in different pulmonary conditions. The prototype is not clinically validated and must not guide diagnosis or treatment.
