# Notebooks

This directory contains the Jupyter notebooks used to reproduce the New York City XCrime-LLM workflow, including preprocessing, feature engineering, training-data preparation, fine-tuning data generation, test inference and evaluation, and SHAP-based explainability.

## Included Notebooks

1. `01_preprocessing_and_feature_engineering.ipynb`
   Prepares the NYC crime data, constructs the spatial grid, engineers the spatio-temporal features, creates the seven-day prediction labels, and generates the chronological train, validation, and test splits.

2. `02_create_training_subset.ipynb`
   Creates the 30% training subset used for the XCrime-LLM fine-tuning workflow.

3. `03_create_fine_tuning_jsonl.ipynb`
   Converts the training subset and validation data into the JSONL format used for supervised fine-tuning.

4. `04_test_inference_and_evaluation.ipynb`
   Runs inference on the NYC test split and computes the prediction and latency metrics used for evaluation.

5. `05_shap_explainability.ipynb`
   Performs the SHAP-based explainability analysis for the selected crime event type and generates global and local feature-attribution results.
