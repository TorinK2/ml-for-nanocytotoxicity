This reposity stores the code for Torin Kovach's NanoBioTech project, "Towards a More General, Better Understood *in 
silico* Model of Nanoparticle Cytotoxicity."

A short summary of what the files contain:
- `raw_datasets` Data collected from the literature on cytotoxicity modeling of nanomaterials.
- `compiled_datasets` Compiled, cleaned, and organized version of the raw_datasets, for viewing and statistical analysis.
- `normalize_data.ipynb` Python notebook which reads in the raw datasets and compiles and cleans them into a single dataset, `compiled_datasets/complete_nanotox_dataset.csv`
- `preprocess_data.ipynb` Python notebook which reads in the compiled dataset and prepares it (e.g., one-hot encodings of categorical features) for statistical analysis, `compiled_datasets/nanotox_features_dataset.csv`
- `simple_ml_predictions.ipynb` Python notebook which creates a simple train/test split over our dataset, trains a random forest model, estimates accuracy metrics, and generates ROC curve.
- `feature_importance.ipynb` Python notebook which computes feature importance metrics over the dataset and saves resulting plots. Specifically, random forest mean decrease in impurity and SHAP values are computed.
- `compare_full_to_within.ipynb` Python notebook which demonstrates a restrained example of generalization across feature testing, as described in "Generalization across assays, cell types, NP types, etc." section of the final report.
- `figures` Feature importance features generated and saved for the report.
