# Lab11: Hyperparameter Tuning and AutoML

## What I Did
- Explored hyperparameters for Random Forest, Logistic Regression and Support Vector Macine models with defaults.
- Manual tuning Random Forest (max_depth 2-10, n_estimators 10-200; best acc 0.95; heatmap).
- Grid Search RF (params: depth 4-8, est 50-150, features auto/sqrt; best acc 0.89 CV, 0.93 test).
- Random Search RF (20 iter, CV=5; best {'depth':12, 'features':None, 'est':198}; acc 0.93 test).
- AutoML with AutoGluon (60s limit; leaderboard, best WeightedEnsemble 0.93 acc).

## What I Learned
- Hyperparameters are set before pre-training to control for complexity.
- Cross Validation with reliable estimation vs single split; 5 was used for tuning.
- AutoML: Automates selection/tuning; quick baselines, handles ensembles.

## Challenges
- Compute constraints; short time_limit in AutoML—balanced iterations to avoid timeouts, emphasizing resource management.
- Overall, tuning boosts performance but requires strategy—gained appreciation for AutoML in iterative workflows.
