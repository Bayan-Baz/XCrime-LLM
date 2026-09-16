# XCrime-LLM

Official implementation of **XCrime-LLM: An Explainable Spatio-Temporal Crime Prediction Framework**

## 📄 Paper

**XCrime-LLM: An Explainable Spatio-Temporal Crime Prediction Framework**  
*Computers*, 2026, 15(5), 325.

🔗 [Read the published paper](https://doi.org/10.3390/computers15050325)

## Overview

XCrime-LLM is an explainable large language model-based framework for spatio-temporal crime prediction. It combines engineered spatio-temporal features, schema-guided prompting, supervised fine-tuning, and explainability to support region-level crime prediction.

The framework predicts whether each of four felony categories—Burglary, Robbery, Grand Larceny, and Felony Assault—will occur within the next seven days for a given spatial region.

## Features

XCrime-LLM uses seven spatio-temporal features:

- `last7_total` – total number of crimes during the previous 7 days
- `last28_mean` – mean crime count during the previous 28 days
- `recency` – time since the most recent crime occurrence
- `base_rate` – historical crime occurrence rate
- `R1_influence` – influence from neighboring regions
- `dow` – day of the week
- `month` – month of the year
