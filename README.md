### Cardiovascular Disease Prediction with Machine Learning, RFECV with StratifeidKFold, Ensemble Techniques, and XAI - SHAP & LIME 

This project implements an end‑to‑end machine learning pipeline for cardiovascular risk prediction using a clinical dataset of **over 68,000 patient records** and **17 clinical and lifestyle‑related features**. The workflow includes:

- **Data Preprocessing**: Removal of non‑contributing columns, handling of outliers, calculation of BMI and blood‑pressure categories, and stratified train‑test split (80:20).  
- **Feature Selection**: Recursive Feature Elimination with Cross‑Validation (RFECV) to identify an optimal subset of **14 discriminative risk factors**.  
- **Model Evaluation**: Comprehensive comparison of multiple classifiers, including **Logistic Regression, Decision Tree, Random Forest, K‑Nearest Neighbors**, and advanced gradient‑boosting methods (**XGBoost, LightGBM, CatBoost, Gradient Boosting, AdaBoost**), culminating in **CatBoost** as the best‑performing single model (ROC‑AUC ≈ 0.8086).  
- **Stacking Ensemble**: Construction of a **Stacking‑V1 classifier** (LR+DTC+RF+KNN) with a **LogisticRegression meta‑learner**, achieving an ROC‑AUC of **0.7924** on the RFECV‑selected features.  
- **Explainable AI (XAI)**: Integration of **SHAP** for global feature‑importance analysis and **LIME** for local, instance‑wise explanations on the Stacking‑V1 model, enabling transparent, interpretable cardiovascular risk predictions suitable for clinical‑decision support.

The project showcases the application of ensemble learning and XAI to high‑volume medical data for early intervention and model interpretability, with ongoing work focused on feature‑importance‑driven refinement and hyperparameter tuning to improve performance toward a production‑ready system.
