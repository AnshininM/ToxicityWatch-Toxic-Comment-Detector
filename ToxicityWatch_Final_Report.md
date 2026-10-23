# ToxicityWatch: Toxic Comment Detector
## Final Project Report

**Generated:** 23 October 2026, 05:49 AM

## 1. Project Overview
ToxicityWatch is a machine-learning prototype that classifies comments
as toxic or non-toxic using a custom Transformer model.

## 2. Objective
To build and evaluate a text-classification workflow and analyze
the model's errors.

## 3. Dataset
Source: Hugging Face `SetFit/toxic_conversations`.

Dataset files are not included in the GitHub repository because
the dataset license has not yet been verified.

## 4. Model Architecture
- Transformer encoder layers: 2
- Embedding dimension: 128
- Attention heads: 4
- Feed-forward dimension: 256
- Maximum sequence length: 128 tokens
- Approximate parameters: 2.84 million
- Training epochs: 4

## 5. Held-out Test Results

| Metric | Result |
|---|---:|
| Accuracy | 85.25% |
| Macro F1-score | 59.45% |
| Toxic precision | 22.25% |
| Toxic recall | 34.67% |

These results describe the underlying Transformer model.

## 6. Error Analysis
The model can misclassify comments, including compliments and threats.
Precision, recall, and F1-score help reveal limitations that accuracy
alone may not show.

## 7. Hybrid Prediction Prototype
A supplementary function combines the model with limited rule-based
safeguards for selected positive phrases and explicit threats. It passed
8 of 8 selected manual sanity tests. This small hand-picked test is not
a measure of overall model accuracy.

## 8. Limitations
- False-positive and false-negative predictions may occur.
- Rule-based safeguards cover only selected phrases.
- The test metrics above do not evaluate the hybrid function.
- The prototype should not be the sole basis for moderation decisions.

## 9. Conclusion
ToxicityWatch demonstrates Transformer-based text classification,
evaluation, error analysis, and a limited hybrid prediction prototype.
Broader validation and further model improvements are needed.

## 10. Repository
https://github.com/AnshininM/ToxicityWatch-Toxic-Comment-Detector
