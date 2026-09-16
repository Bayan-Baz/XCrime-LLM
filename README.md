# XCrime-LLM

Official implementation of **XCrime-LLM: An Explainable Spatio-Temporal Crime Prediction Framework**.

XCrime-LLM is an explainable large language model (LLM)-based framework for **spatio-temporal crime prediction**. It combines engineered spatio-temporal features, schema-guided prompting, supervised fine-tuning, structured multi-label prediction, and **KernelSHAP-based explainability** for region-level crime occurrence prediction.

This repository provides the New York City (NYC) preprocessing, feature-engineering, fine-tuning data preparation, test inference and evaluation, and SHAP explainability workflow used for XCrime-LLM.

## 📄 Paper

**B. Baz, A. Attiah, A. Hakeem, and N. M. Almani,  
“XCrime-LLM: An Explainable Spatio-Temporal Crime Prediction Framework,”**  
*Computers*, 2026, 15(5), 325.

🔗 [Read the published paper](https://doi.org/10.3390/computers15050325)

## Overview

XCrime-LLM predicts whether each of four felony categories—Burglary, Robbery, Grand Larceny, and Felony Assault—will occur within the next seven days for a given spatial region.

The framework combines:

- spatio-temporal feature engineering
- schema-guided prompting
- supervised fine-tuning
- structured multi-label crime occurrence prediction
- KernelSHAP-based feature attribution

## Features

XCrime-LLM uses seven spatio-temporal features:

- `last7_total` – total number of crimes during the previous 7 days
- `last28_mean` – mean crime count during the previous 28 days
- `recency` – time since the most recent crime occurrence
- `base_rate` – historical crime occurrence rate
- `R1_influence` – influence from neighboring regions
- `dow` – day of the week
- `month` – month of the year
