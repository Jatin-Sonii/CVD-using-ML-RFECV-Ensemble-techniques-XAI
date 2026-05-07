# Cardiovascular Disease (CVD) Prediction with Stacking Ensemble and XAI

This project develops a robust predictive framework for Cardiovascular Disease (CVD) detection using an advanced stacking ensemble methodology. The aim is to combine strong predictive performance with clear, interpretable explanations suitable for clinical decision‑making support.

## Overview

- Trains and evaluates five baseline models: Decision Tree (DT), Logistic Regression (LR), Gaussian Naive Bayes (GNB), Random Forest (RF), and K‑Nearest Neighbors (KNN).
- Uses **Stratified 5‑Fold Cross‑Validation** to ensure stable and reliable performance estimates across diverse data splits.
- Optimizes model hyperparameters using **Optuna**, a Bayesian optimization framework, to fine‑tune each baseline for peak accuracy.

## Ensemble Architecture

- Builds a **Stacking Ensemble Tournament** with five distinct architectural variants (V1–V5), where base model predictions are used as inputs for various meta‑learners.
- Systematically compares ensemble versions to identify the configuration that maximizes predictive performance while maintaining robustness.

## Explainable AI (XAI)

To ensure the model is not a “black‑box” and remains clinically interpretable:

- Uses **SHAP (SHapley Additive exPlanations)** for:
  - Global feature importance analysis.
  - Beeswarm plots to visualize primary CVD risk drivers.
- Applies **LIME (Local Interpretable Model‑agnostic Explanations)** for:
  - Instance‑level explanations of individual patient predictions.
  - Human‑readable, local justifications that support clinical trust.

This combination of high‑performance stacking ensembles and dual‑layer XAI provides a transparent, accurate, and clinically meaningful CVD prediction system.
