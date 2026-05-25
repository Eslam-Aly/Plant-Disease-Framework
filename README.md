# Plant-Disease-Framework

An uncertainty-aware and explainable deep learning framework for robust plant disease diagnosis under real-world agricultural conditions.

This repository contains the experimental outputs, evaluation pipelines, and supporting artifacts for the research project:

> **“Uncertainty-Aware and Explainable Plant Disease Diagnosis Framework for Real-World Agricultural Deployment”**

The framework investigates the reliability, robustness, explainability, calibration quality, deployment suitability, and decision safety of deep convolutional neural network architectures under controlled and real-world conditions.

---

# Overview

The proposed framework extends traditional CNN-based plant disease classification by integrating:

- Cross-dataset robustness evaluation
- Synthetic perturbation analysis
- Monte Carlo Dropout uncertainty estimation
- Confidence calibration
- Grad-CAM explainability
- Rule-based expert decision support
- Deployment-oriented benchmarking
- User-centered trust and usability evaluation

The repository focuses on evaluating how agricultural AI systems behave beyond benchmark accuracy when exposed to real-world deployment challenges.

---

# Evaluated Architectures

The following pretrained CNN backbones were evaluated:

- ResNet50
- EfficientNet-B0
- MobileNetV2

All models were trained using transfer learning with ImageNet-pretrained weights.

---

# Datasets

The framework uses:

## PlantVillage
Controlled-environment plant disease dataset with clean backgrounds and standardized imaging conditions.

## PlantDoc
Real-world plant disease dataset containing:
- background clutter,
- lighting variability,
- occlusions,
- field-condition complexity.

Cross-dataset evaluation was performed by training on PlantVillage and testing on PlantDoc.

---

# Research Objectives

The framework investigates:

1. Cross-dataset generalization
2. Robustness under synthetic perturbations
3. Predictive uncertainty estimation
4. Calibration reliability
5. Explainability consistency
6. Deployment efficiency trade-offs
7. Human-centered trust and usability

---

# Repository Structure

```text
Plant-Disease-Framework/
│
├── 01_train_backbones_outputs/
│   Backbone training outputs and baseline evaluation results
│
├── 02_rq1_cross_dataset_outputs/
│   Cross-dataset evaluation outputs and figures
│
├── 03_rq2_robustness_outputs/
│   Robustness evaluation under perturbations
│
├── 04_rq3_uncertainty_expert_system_outputs/
│   Uncertainty estimation, calibration, and expert-system outputs
│
├── 05_rq4_explainability_outputs/
│   Grad-CAM explainability analysis outputs
│
├── 06_rq5_deployment_outputs/
│   Deployment benchmarking and efficiency evaluation
│
├── 07_rq6_ablation_outputs/
│   Ablation study outputs
│
├── 08_rq7_user_study_outputs/
│   User trust and usability evaluation outputs
│
└── metadata/
    Supporting metadata and experiment configuration files
```

---

# Experimental Components

## Backbone Training and Baseline Evaluation
- Transfer-learning-based CNN training
- Controlled benchmark evaluation
- Baseline accuracy and F1-score analysis

## Cross-Dataset Evaluation
- PlantVillage → PlantDoc transfer analysis
- Accuracy degradation measurement
- Generalization gap evaluation

## Robustness Evaluation

Synthetic perturbations:
- Blur
- Low-light
- Occlusion
- Background clutter

Multiple severity levels were evaluated.

## Uncertainty Estimation

Implemented using:
- Monte Carlo Dropout
- Predictive entropy
- Temperature scaling calibration

Metrics:
- Expected Calibration Error (ECE)
- Predictive entropy
- High-confidence misclassification rate

## Explainability

Grad-CAM was used to:
- visualize model attention,
- measure leaf-focused attention,
- analyze background leakage.

## Expert Decision Layer

The framework transforms predictions into actionable outputs:
- Accept
- Monitor
- Retake
- Expert review

based on confidence and uncertainty thresholds.

## Deployment Evaluation

Deployment-oriented metrics include:
- Model size
- Parameter count
- Inference latency
- End-to-end pipeline time
- Deployment suitability ranking

## User Study

The deployed prototype was evaluated using:
- trust scores,
- usability assessment,
- clarity evaluation,
- perceived safety,
- interface preference analysis.

---

# Technologies

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# Hardware Environment

Experiments were conducted using GPU-accelerated environments for training and inference benchmarking.

---

# Research Supervision

## First Supervisor
**Prof. Dr. Raja Hashim Ali**

## Second Supervisor
**Prof. Dr. Iftikhar Ahmed**

## Co-Author
**Dr. Mohammed Nazeh Alimam**

---

# Citation

If you use this repository or reference the framework, please cite the associated research work.


---

# Author

**Eslam Aly**  
Software Engineer | AI Enthusiast

- GitHub: https://github.com/Eslam-Aly
- LinkedIn: https://www.linkedin.com/in/eslam-aly
- Portfolio: eslamaly.com

---

# License

This repository is provided for research and educational purposes.
