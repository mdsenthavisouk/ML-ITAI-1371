# Lab10: Unsupervised Learning on Titanic

## What I Did
- Used preprocessed Titanic features (without Survived; e.g., Age, Fare, FamilySize).
- Applied K-Means (k=2, random_state=42, n_init=10); clusters: 726/165 passengers, inertia 4516.68.
- Compared clusters vs survival: Crosstab (Cluster 0: 474 died/252 survived; Cluster 1: 75/90); rates 34.7%/54.5%.
- Elbow method: Tested k=1-10, plotted inertia; bend at k=2-3.

## What I Learned
- K-Means: Groups by similarity; inertia measures compactness (lower better).
- Elbow: Helps select optimal k where adding clusters yields diminishing returns.

## Challenges
- Feature selection; no labels—challenged by potential noise, emphasized scaling/engineering for meaningful clusters.
- Interpreting clusters; alignment with survival intriguing but coincidental—learned unsupervised's exploratory nature, needing domain knowledge.
