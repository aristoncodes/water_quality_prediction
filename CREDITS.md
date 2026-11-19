# Credits

## Original authors

This project was designed and built by the following team. All code, notebooks, results,
the report and the presentation in this repository are their work.

Original repository: [github.com/Taj-2005/water_quality_prediction](https://github.com/Taj-2005/water_quality_prediction)

| Author | GitHub | What they built |
| :--- | :--- | :--- |
| Shaik Tajuddin *(team lead)* | [@Taj-2005](https://github.com/Taj-2005) | Repository setup, `src/config.py`, data dictionary, `src/clean.py`, cleaning and EDA notebooks; Phase 2 NN data prep and regularization study |
| Parthraj Singh Bhati | [@parthrajsinghbhati](https://github.com/parthrajsinghbhati) | Target definition, `src/split.py`, `src/preprocess.py`, `src/evaluate_api.py`, `src/evaluation.py`, `src/run_evaluation.py`, final evaluation; Phase 2 deep learning foundation (`src/dl/`) |
| Himanshu Pandey | [@14-himanshu](https://github.com/14-himanshu) | Literature review, `src/features.py`, `src/models_rf.py`, Random Forest notebook; Phase 2 base MLP and architecture study |
| Jivit Rana | [@Jivit87](https://github.com/Jivit87) | `src/models_xgb.py`, XGBoost notebook, Optuna tuning, ablation |
| Satya Yadav | [@ACE-pwd](https://github.com/ACE-pwd) | `src/metrics.py`, naive baseline notebook, IEEE report, presentation, viva prep |

## Study and presentation split (Phase 1)

The team below is studying this project and presenting its Phase 1 work. Each person
covers the parts listed, building on the original authors' work above.

| Presenter | Builds on work by | Covers | Files | Viva theory topic |
| :--- | :--- | :--- | :--- | :--- |
| Jigyasu | Shaik Tajuddin | Repo setup, config, data dictionary, cleaning, EDA | `src/config.py`, `src/clean.py`, `docs/data_dictionary.md`, `notebooks/01_cleaning`, `02_eda`, `tests/test_clean.py` | Missing data, duplicates, impossible values, the median-imputation finding |
| Manya | Parthraj Singh Bhati, Himanshu Pandey (features) | Target definition, leakage-safe split, preprocessing, feature engineering | `docs/target_definition.md`, `src/split.py`, `src/preprocess.py`, `src/features.py`, `src/evaluate_api.py`, `tests/test_split.py`, `test_preprocess.py`, `test_features.py` | CCME formula, data leakage, area-grouped split, fitting on train only |
| Satyam | Himanshu Pandey (RF), Jivit Rana | Random Forest, XGBoost, tuning, ablation | `src/models_rf.py`, `src/models_xgb.py`, `notebooks/04_random_forest`, `05_xgboost`, `reports/rf_results.csv`, `xgb_results.csv`, `xgb_ablation.csv` | Bagging vs boosting, Optuna tuning, early stopping |
| Aditya | Satya Yadav, Parthraj Singh Bhati (evaluation) | Metrics, naive baseline, final evaluation, SHAP, report and presentation | `src/metrics.py`, `src/evaluation.py`, `src/run_evaluation.py`, `notebooks/03_naive_baseline`, `06_evaluation`, `results/`, `report/`, `presentation/` | MAE/RMSE/R², baseline, SHAP, the partial-measurement result (R² 0.9997 → 0.834 → 0.573) |
