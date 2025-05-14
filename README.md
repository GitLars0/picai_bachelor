# Prostate Cancer Detection Using Radiomics, Clinical Guidelines & Language Models

This repository contains a structured pipeline for prostate cancer lesion characterization based on MRI radiomics, clinical guideline-based prompts, and large language model embeddings (e.g., BioBERT). The pipeline covers data preprocessing, feature extraction, embedding generation, and performance evaluation using traditional machine learning classifiers.

---

## 📁 Project Structure

- **Preprocessing.ipynb**  
  Handles image resampling and preprocessing steps (e.g., intensity normalization, spatial alignment).

- **feature_extraction.ipynb**  
  Extracts radiomic features from resampled MRI images, generates clinical guideline-based textual prompts, selects relevant features, and rounds them for stability and interpretability.

- **Embedding_extraction.ipynb**  
  Converts text prompts into embeddings using pretrained language models (e.g., BioBERT), trains machine learning models (e.g., Logistic Regression), and evaluates performance using metrics such as accuracy, AUC, and balanced accuracy.

- **plotting.ipynb**  
  Generates visualizations (e.g., performance bar plots with confidence intervals) for comparative model analysis.

---

## 🧠 Key Components

- **Radiomics**: Quantitative features extracted from MRI images using PyRadiomics or equivalent.
- **Clinical Prompts**: Domain-informed prompt templates linking radiomic features to PI-RADS-like descriptors.
- **Embeddings**: Generated using pretrained models like BioBERT to encode prompt semantics.
- **ML Pipeline**: Logistic regression or other classifiers trained on feature/embedding representations.
- **Evaluation**: Includes train/test splitting, accuracy, ROC AUC, and balanced accuracy metrics.
