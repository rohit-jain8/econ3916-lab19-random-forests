# econ3916-lab19-random-forests
# Tree-Based Models: Random Forests

## Objective

I compared models for predicting house values in the California Housing dataset and looked at which features mattered most to the random forest's predictions.

## Methodology

- I fit a single decision tree, OLS, Ridge, and a random forest on the same training data and compared their test R² values.
- I compared mean decrease in impurity (MDI) and permutation importance for the random forest.
- I used cross-validation to tune the forest's maximum depth and the number of features it could consider at each split.
- I wrote a prompt asking AI for a feature importance chart, went through two rounds, and checked the results against my notebook.

## Key Findings

- The decision tree had a test R² of 0.6228, Ridge had 0.5758, and the random forest had 0.8046. After tuning, the forest's test R² went up to 0.8094.
- Latitude scored 0.0890 by MDI and 0.4427 by permutation importance. It ranked higher by permutation importance, where shuffling it led to a relatively large drop in test R².
- Both AI rounds matched the notebook's permutation importance values and feature order. In the second round, I asked for R² to be set explicitly and checked that the chart's bars matched the table.
