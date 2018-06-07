# EuroPOND-model-comparison
Comparing disease staging across the models developed by partners in the EuroPOND consortium

## EuroPOND models
| Model | Team | Person(s) |
|:----- |:----:|:---------:|
| EBM   | UCL  | Neil, et al. |

- dEBM (Vikram)
- SuStaIn (Alex, UCL)
- DEM (Neil)
- Gaussian Process regression (Marco => Inria Sophia)
- Network model 1: dynamics on networks (Igor)
- Network model 2: dynamics of networks (Sara/Neil)
- Spatiotemporal 1: longitudinal shape (Alexandre: Deformetrica)
- Spatiotemporal 2: Bayesian ME (Igor: LeasPy)
- Spatiotemporal 3: Vertex clustering trajectories (Raz, UCL)
- Linear ME models (Eline)
- Off-the-shelf machine learning: classifiers
  - Need volunteer(s) to do this
  - Point: for comparison with AUC for clinical classification

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
