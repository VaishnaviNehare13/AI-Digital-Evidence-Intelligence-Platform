# AI Digital Evidence Intelligence Platform

An AI-powered digital forensic platform designed to analyze and verify
different forms of digital evidence using artificial intelligence and
deep learning.

## Project Overview

The platform combines multiple AI-based approaches to support intelligent
analysis of digital evidence.

### Main Components

1. **Legal Document Anomaly Detection**
   - Detects unusual or anomalous sections in legal documents.
   - Uses an Autoencoder-based approach.
   - Reconstruction error is used to identify unusual content.

2. **AI-Generated Image Evidence Analysis**
   - Determines whether an image is REAL or AI-GENERATED/FAKE.
   - Uses a ResNet-18 deep learning model.
   - Supports forensic analysis of synthetic images.

## Image Forensics

The image-forensics module uses ProGAN and CIFAKE datasets.

### Dataset

- REAL images
- AI-GENERATED/FAKE images
- Mixed-source training for improved generalization

### Model

**ResNet-18**

Input:
`224 × 224 RGB image`

Output:
`REAL / FAKE`

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC

## Results

The initial improved ResNet-18 achieved:

| Metric | Result |
|---|---:|
| Test Accuracy | 94.10% |
| Precision | 95.53% |
| Recall | 92.53% |
| F1-Score | 94.01% |
| ROC-AUC | 0.9837 |

The model was also evaluated on an independent CIFAKE dataset to
investigate cross-dataset generalization.

## Project Structure

```text
AI-Digital-Evidence-Intelligence-Platform/
│
├── README.md
├── notebooks/
├── models/
├── results/
├── requirements.txt
└── .gitignore
