# "Modern" Data Science Good Practices

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-disabled)](https://www.linkedin.com/in/everestlaw/)

## Overview

This project demonstrates a modern, end-to-end data science workflow using publicly available datasets. The goal is to build a robust and understandable model while highlighting key data science skills.

## Key Skills Demonstrated
In addition to LLM-assisted coding———

*  **Reproducibility through [Poetry](https://python-poetry.org/):** Locked down all dependencies to ensure consistent builds. Poetry also allows us to easily add/update/remove dependencies.

*   **Hyperparameter Optimization with [Optuna](https://optuna.org/):** Tuned the CatBoostClassifier hyperparameters using Optuna's [TPE sampler](https://hub.optuna.org/samplers/tpe_tutorial/), which is much more efficient than exhaustive grid search.

*   **Model Interpretability with [SHAP](https://shap.readthedocs.io/en/latest/example_notebooks/overviews/An%20introduction%20to%20explainable%20AI%20with%20Shapley%20values.html):**  Utilized SHAP (SHapley Additive exPlanations) values to understand the model's decision-making process and identify key drivers of predictions.
*   **Best Practices in Common Libraries**  Enabled [copy_on_write](https://pandas.pydata.org/docs/user_guide/copy_on_write.html#copy-on-write) in pandas to reduce memory footprint, used [pyarrow](https://pandas.pydata.org/docs/user_guide/pyarrow.html) wherever possible ...


## Project Tech Stack

*   **Programming Language:** Python 3.12
*   **Libraries:** pandas, matplotlib, plotly, optuna, seaborn, shap, catboost, scikit-learn
*   **Dataset:** 
    - [Loan Approval Classification Dataset](https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data/data) (Kaggle, binary classification)
*   **Main Executables:**
    - [binary_classification.ipynb](binary_classification.ipynb)

## Getting Started

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME
    ```
2.  **Install dependencies and activate environment:**
    ```bash
    poetry install  # reading from poetry.lock
    poetry env activate # provides a shell command that activates a virtual env
    ```
3.  **Explore :** Open one of the notebooks and follow the detailed comments within!


## Further Exploration
*   Experiment with feature selection and engineering techniques.
*   Try different machine learning algorithms.
*   Deploy the model to e.g., [GCP Cloud Run](https://cloud.google.com/run?hl=en) for scalability.