# mlb-player-data-analysis

Exploratory Data Analysis: MLB Player Performance, Salary and Demographics
Project overview
This project explores a Major League Baseball (MLB) player dataset to investigate relationships between player demographics, career performance, experience and salary.

Using Python, I conducted exploratory data analysis, statistical hypothesis testing and multiple linear regression to identify patterns in the data, examine relationships between variables and assess how much salary variation the selected model explains.
Questions explored
Is player race associated with playing position in this dataset?
How are offensive performance metrics associated with salary?
How do salaries compare between player groups with different levels of games played, while using a threshold for hits per game?
Which selected variables are statistically significant in an OLS salary model?
Tools
Python, pandas, NumPy, SciPy, statsmodels, Matplotlib and Bokeh.
Methods
Data cleaning and missing-value checks
Descriptive statistics and visual exploration
Chi-square test of independence
Spearman rank correlation
Independent-samples t-test
Multiple linear regression using OLS
Residual diagnostics
Selected visualisations
Player race and playing position

Career home runs and walks

Hits per game and salary

Key findings
A chi-square test found a statistically significant association between player race and playing position in the analysed sample (p < 0.001). This describes an association and does not explain its causes.
Career home runs and career walks showed a strong positive monotonic association (Spearman's rho approximately 0.819).
Hits per game and salary showed a positive monotonic association (Spearman's rho approximately 0.634).
An independent-samples t-test found a statistically significant salary difference between two groups selected using thresholds for hits per game and games played (p < 0.001). This comparison does not isolate the causal effect of experience.
The final OLS model included team payroll, hits per game, career home runs and career runs. Its adjusted R² was approximately 0.493, meaning it explained around 49.3% of salary variation in the analysed sample after accounting for the number of predictors.
Limitations
The model does not include every potential determinant of salary.
Statistical associations do not establish causation.
The t-test compares selected groups and does not hold every other factor constant.
The model's explanatory performance does not by itself establish predictive accuracy on unseen data; no separate test set or cross-validation was used.
Findings reflect the dataset supplied for the university module and may not generalise to current MLB conditions.
Repository contents
MLB_EDA_Portfolio.ipynb — notebook containing the analysis and visualisations.
mlb.csv — dataset used in the analysis.
images/ — selected chart images embedded in this README.
Running the notebook
Ensure Python and the packages imported in the notebook are installed.
Place mlb.csv in the same directory as MLB_EDA_Portfolio.ipynb.
Open the notebook in Jupyter Notebook, JupyterLab or a compatible environment.
Run the cells from top to bottom. The selected Matplotlib charts are saved to the images/ directory.

Dataset note: mlb.csv is included in this repository package so the analysis can be reproduced. Before publishing the repository publicly, make sure the dataset’s terms permit redistribution, particularly because it was supplied as part of a university module.
Project context
Completed as part of the Software Analytics module of my MSc in Business Analytics at Aston University. Project mark: 78.37%.
