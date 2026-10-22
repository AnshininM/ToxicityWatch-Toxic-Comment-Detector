# ToxicityWatch: Toxic Comment Detector

## Overview
ToxicityWatch is a prototype that classifies comments as toxic or non-toxic using a custom Transformer model.

## Features
- Text classification using a trained Transformer
- Evaluation metrics, confusion matrix, and training history
- Error analysis and prediction testing
- Hybrid prediction function with limited rule-based safeguards for selected positive phrases and explicit threats

## Test Results
Results from the existing held-out test evaluation:
- Test samples: 50,000
- Accuracy: 85.25%
- Macro F1: 59.45%
- Toxic precision: 22.25%
- Toxic recall: 34.67%

## Sanity Testing
The hybrid prediction function passed 8 of 8 selected manual sanity tests.
This is a small, hand-picked test and does not represent generalization accuracy.

## Limitations
The model can misclassify comments, including compliments and threats.
Rule-based safeguards handle only selected phrases and do not solve general classification errors.
The reported test metrics describe the underlying model, not the hybrid prediction function.

## Repository Contents
- Notebook: project workflow and experiments
- artifacts/: trained model, vocabulary, labels, and configuration
- results/: evaluation metrics, confusion matrix, training history, and error analysis

## Dataset and Reproducibility
The source dataset is SetFit/toxic_conversations on Hugging Face.
The dataset license has not yet been verified, so dataset files are not included in this repository.
Consult the notebook and results/source_manifest.json for source and preparation details.

## Disclaimer
This is an educational prototype and should not be used as the sole basis for moderation decisions.
