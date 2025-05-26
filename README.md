# UU-APB-Exam
UU Applied Pharmaceutical Bioinformatics Final Exam - May 2025

## Objective
You are given a dataset of small molecules and their biological activity (𝐾𝑖, in 𝑛𝑀). Your task is to explore the data, build regression and classification models, evaluate them, and reflect on your modelling process and results.

## Instructions
Submit a PDF report. Code is optional but encouraged as an appendix or separate file.

1. Data Exploration
- Load and inspect the dataset.
- Analyse the distribution of 𝐾𝑖 and decide whether to apply a log-transformation (e.g., log10(𝐾𝑖)). Justify your choice and apply it if appropriate.

2. Descriptor Preparation
- Generate suitable molecular descriptors (e.g., ECFP4, RDKit descriptors).
- Justify your descriptor choices.

3. Descriptor Space Visualization
- Use at least one dimensionality reduction method (e.g., PCA, t-SNE, UMAP).
- Highlight clustering or separation of actives/inactives.
- Comment on how structurally diverse the dataset appears based on clustering or spread in the projected space.
- Optionally compare multiple methods.

4. Modelling
- Use and compare at least three machine learning methods for each task.
  1. Regression
    - Build and evaluate regression models using 10-fold cross-validation.
    - Report 𝑅2 and 𝑀𝑆𝐸.
  
  2. Classification
    - Choose at least two thresholds for active/inactive classification. Try to make one chemically meaningful value (e.g., 𝐾𝑖 < 1000 nM) and one which gives a more unrealistic but balanced setup.
    - For each threshold:
    – Train three models using descriptors.
    – Evaluate with 10-fold cross-validation (CV).
    – Report AUC, precision, recall, F1-score.
    – Reflect on how thresholds affect class balance, interpretability and usefulness.

5. Discussion
- Compare model performance and metric outcomes.
- Discuss effects of descriptor relevance, threshold impact, and class imbalance.

6. Report Format
- Recommended structure:
  1. Introduction
  2. Methods
  3. Results
  4. Discussion
  5. Conclusion
- Suggested length: 4–6 pages.

7. Submission
- Submit your PDF report.
- Code is optional but encouraged.
