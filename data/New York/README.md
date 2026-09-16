# New York City Data

This directory contains the New York City data and derived files used in the XCrime-LLM experiments.

## Files

- `NYC_Crime.csv` — NYC crime data used as input to the preprocessing and feature-engineering pipeline.

- `region_cells.csv` — spatial grid definition linking region IDs to the 2 km grid cells used in the study.

- `NYC_splits.zip` — processed chronological dataset splits used in the experiments, including the training, validation, and test sets.

- `fine_tuning.zip` — JSONL datasets prepared for the XCrime-LLM fine-tuning workflow.

The preprocessing, feature-engineering, data preparation, inference, and explainability workflows are provided in the `notebooks/` directory.
