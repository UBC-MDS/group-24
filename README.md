# Adult Income Predictor

- Author: Michael Suriawan, Francisco Ramirez, Tingting Chen, Quanhua Huang

Adult Income Predictor project, a data analysis project for DSCI 522 (Data Science workflows) course in the Master of Data Science program at the University of British Columbia.

## About

This report presents the application of a K-Nearest Neighbors (KNN) Classifier to predict an individual's annual income based on selected categorical socioeconomic features from the Adult dataset. The dataset, sourced from the 1994 U.S. Census Bureau, contains 48,842 instances and features such as age, education, occupation, and marital status. The model achieved an accuracy of approximately 80%, with a tendency to predict more individuals with incomes below \$50K compared to those above. This result emphasizes the importance of socioeconomic factors in determining income levels. Further investigation into individual feature contributions and the inclusion of numerical variables like age and hours-per-week could enhance prediction performance.

## Dataset

The Adult dataset, originally curated from the 1994 U.S. Census Bureau database, is a well-known benchmark dataset in machine learning. Its primary objective is to predict whether an individual earns more or less than \$50,000 annually based on various demographic and socio-economic attributes. With 48,842 instances and 14 features, the dataset encompasses a mix of categorical and continuous variables, making it a rich resource for classification tasks and exploratory data analysis.

The Key features used in this project are:

- Age
- Education Level
- Marital Status
- Occupation
- Race
- Sex
- Relationship
- Hours Worked per Week

The target variable is whether an individual's income exceeds \$50,000 per year.

It was sourced from the UCI Machine Learning Repository and can be found [here](https://archive.ics.uci.edu/dataset/2/adult)

## Report

The final report can be found [here](notebooks/adult_income_predictor_report.pdf).

## Usage

First time running the project, run the following from the root of this repository:

``` bash
conda-lock install --name adult-income-predictor conda-lock.yml
```

To run the analysis, run the following from the root of this repository:

``` bash
jupyter lab 
```

Open `notebooks/adult_income_predictor_report.ipynb` in Jupyter Lab and under Switch/Select Kernel choose "Python \[conda env:adult-income-predictor\]".

Next, under the "Kernel" menu click "Restart Kernel and Run All Cells...".

## Dependencies

- `conda` (version 23.9.0 or higher)
- `conda-lock` (version 2.5.7 or higher)
- `jupyterlab` (version 4.0.0 or higher)
- `nb_conda_kernels` (version 2.3.1 or higher)
- Python and packages listed in [`environment.yml`](environment.yml)

## License

The Adult Income Predictor report contained herein are licensed under the [Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License](https://creativecommons.org/licenses/by-nc-sa/4.0/). See [the license file](LICENSE.md) for more information. If re-using/re-mixing please provide attribution and link to this webpage. The software code contained within this repository is licensed under the MIT license. See [the license file](LICENSE.md) for more information.

## References

- Becker, B. & Kohavi, R. (1996). *Adult Dataset*. UCI Machine Learning Repository. <https://doi.org/10.24432/C5XW20>.
- Kolhatkar, V. *UBC Master of Data Science program, 2024-25, DSCI 571 Supervised Learning I*.
- Ostblom, J. *UBC Master of Data Science program, 2024-25, DSCI 573 Feature and Model Selection*.
- Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., et al. (2011). Scikit-learn: Machine Learning in Python. *Journal of Machine Learning Research*, 12, 2825–2830.
