# EuroPOND-model-comparison
Comparing disease staging across the models developed by partners in the EuroPOND consortium

## EuroPOND models
See [this EuroPOND repository](https://github.com/EuroPOND/pond-analysis)

Additional models of interest:
- Ageing trajectories:
  - Leon's [Multi-Task Learning](https://github.com/LeonAksman/bayes-mtl-traj) trajectory model
  - Eline's mixed (efects) models
- Off-the-shelf machine learning classifiers:
  - SVM, MKL, etc.
  - Point: for comparison with AUC for clinical classification
  - Need a volunteer to run this analysis

## Discussion in Paris
- Stratified CV sets. Defined by one person, then shared.
  - Probably don’t need to balance/stratify, due to TADPOLE numbers
- Evaluation measures:
  - Appropriate TADPOLE metrics: AUC for clinical classification, too.
  - (Regression) Correlations between model stages
  - Hold-out longitudinal consistency:
    - "Test" data: N (=200?) individuals having 2x2 timepoints (two disease staging opportunities) each
    - Preferably not those having more than 4, so as not to reduce the data for unsupervised spatiotemporal models (Inserm)

## ACTIONS:
- `Neil`: pre-analysis of numbers for timepoints, etc. in TADPOLE
  - Ideally N=300
  - See Jupyter Notebook in this github repo
- `All`: volunteer for ML classifier task
- `All`: train and test your model
