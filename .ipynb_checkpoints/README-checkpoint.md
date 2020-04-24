# ATMS 597 Project 5 Group A
### Group Members: Chu-Chun Chen, Bowen Fang, David Lafferty
### ASOS Station: Dubuque, Iowa (KDQB)

<b>Task:</b><br>
Using Automated Surface Observation System data from NCDC, build a supervised classification algorithm to predict frozen vs. liquid precipitation type.

<b>Notebooks:</b>
- `DataProcessing`: Parses the METAR data and stores readings for all yeares in a single csv file.
- `LogisticRegression`: Baseline model; scikit-learn's `LogisticRegression` with default parameters.
- `GradientBoostedDecisionTree`: Implementation of sckikit-learn's `GradientBoostingClassifier` including hyperparameter optimisation.
- `RandomForest`: Implementation of sckikit-learn's `RandomForestClassifier` including hyperparameter optimisation.

<b>Results:</b><br>
(All results are for test data)<br>
Baseline model Brier Skill Score: 0.8607<br>
Gradient Boosted Decision Tree Brier Skill Score: 0.9821<br>
Random Forest Brier Skill Score: 0.9845<br>

<b>The best model was the Random Forest, with an improvement of 0.1238 in Brier Skill Score over the basline model!</b>