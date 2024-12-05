# Identifying Entities in Healthcare Data

This project demonstrates the application of Natural Language Processing (NLP) techniques for identifying and extracting entities in healthcare data. Using a labeled corpus, it explores tasks such as tokenization, data preprocessing, exploratory data analysis (EDA), feature extraction, and model building with Conditional Random Fields (CRF). The goal is to identify diseases (D) and treatments (T) effectively.

## Project Workflow

### 1. Workspace Setup
- Import necessary libraries and install required packages to enable NLP and data processing.

### 2. Data Preprocessing
- **Sentence Construction:** Transform individual words into structured sentences using a custom function.
- **Label Analysis:** Analyze and ensure consistency between sentences and their associated labels.

### 3. Exploratory Data Analysis (EDA)
- **Label Distribution:** Observe the quantiles and distribution of labels (D, T, O).
- **Insights:** Highlight the prevalence of "Others" (O) labels in the dataset.

### 4. Concept Identification
- Extract tokens with **NOUN** or **PROPN** PoS tags and analyze their frequency.
- Display the top 25 most common tokens, emphasizing their relevance in healthcare contexts.

### 5. Feature Engineering
- **CRF Features:** Define and compute features for CRF, including word context, capitalization, and more.

### 6. Model Building
- Build a **Conditional Random Field (CRF)** model for entity recognition.
- Train the model on processed data and evaluate it using performance metrics.

### 7. Evaluation
- Predict token labels in the test dataset.
- Calculate the **F1 Score** to measure model performance (achieved score: **0.9086**).

### 8. Named Entity Recognition (NER) for Healthcare
- Identify diseases and treatments using custom NER logic.
- Example: Predict treatments for specific diseases such as *"hereditary retinoblastoma"*.

## Key Results
- **F1 Score:** Achieved a score of 0.9086 for entity recognition.
- Identified treatment for *"hereditary retinoblastoma"* as *"radiotherapy"*.

## Prerequisites
- Python 3.7+
- Libraries: `pandas`, `numpy`, `nltk`, `sklearn-crfsuite`, `matplotlib`
