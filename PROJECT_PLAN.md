# Project Plan

## Project title
AI-Assisted Pneumonia Classification from Lung Ultrasound Images

## Project goal
Build a simple educational computer-vision prototype that classifies lung-ultrasound images into two categories: pneumonia and normal.

## Project question
Can a pretrained image-classification model learn to distinguish pneumonia-associated from normal lung-ultrasound images in a held-out test set?

## Scope
- Begin with image classification, not video diagnosis.
- Use a pretrained model as a baseline.
- Treat predictions as experimental outputs, not medical diagnoses.
- Do not upload patient images or dataset files to this repository.

## Initial workflow
1. Inspect the dataset and document its labels and permitted use.
2. Split data by patient or video before extracting frames.
3. Train a pretrained model on the training set.
4. Use the validation set to make development decisions.
5. Evaluate once on the held-out test set.
6. Build a simple demo only after evaluation.

## Evaluation
Report a confusion matrix, precision, recall, F1-score, and balanced accuracy. Record the patient- or video-level split method and any limitations.

## Safety and limitations
This is an educational research prototype, not a clinically validated medical device. It must not be used to diagnose, treat, or make decisions about a person’s health.
