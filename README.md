# Business Projects
## [Commissions Code System](https://github.com/justin-sharber/Commissions_Code)
A Python-based code system for processing commissions data.  The system automates all calculations and output reports necessary for supporting commissions operations: calculating KPI, auditing and reconciling revenue, calculating sales commissions for sellers.

The system consists of three tiers of code, with the lower tiers providing general data functions and preloading new data in a preferred format, ready for review and substantive calculations.

<img width="500" alt="comp data merge nb head" src="https://github.com/user-attachments/assets/efadf303-223b-4f93-a26a-bb812b5af2a9" />

## [ETL Code System](https://github.com/justin-sharber/ETL-System)
A Python-based code system for preparing data and loading it into the company BigQuery database.  The system coordinates data from 14 different sources with different formats, preprocessing them to exactly match table schemas in the database.  ETL reads from the company data library and imports it with one click.  It uses new file detection so that only recently added files are imported.

<img width="300" alt="etl-flow" src="https://github.com/user-attachments/assets/7df51a58-6673-4a98-a648-b3c00c97137d" />

## [Company Data Pipeline in Google BigQuery](https://github.com/justin-sharber/bigquery-data-pipeline)
A database and pipeline built in the Google Cloud system, which hosts disparate data for multiple partners, with multiple carriers, and heterogeneous formats.  It draws on hundreds of base sheets and contains over one million records.  The database uses a medallion architecture, with raw data stored as close as possible to the original input sources.  A view-based structure causes data to flow from the bronze layer to end dashboards with no manual assistance.

<img width="500" alt="unions-slice" src="https://github.com/user-attachments/assets/1ab5ec62-92c6-4eea-b4ce-bdbbb013855e" />

# Data Science Projects
## [Analysis of Home Mortgage Data](https://github.com/justin-sharber/HMDA)
A project that investigates data from home mortgage applications to predict approvals.  This project has two goals:
1. Predict loan approvals.
2. Test approval rates for unfair discrimination on identity features (race and sex).

To handle high-cardinality features like lender IDs, the analysis introduces an innovative acceptance-rate binning strategy, drastically reducing the size of the encoded feature set.  Machine learning establishhed a baseline accuracy with logistic regression of 69.1% which was not significantly outperformed by other models, establishing an elementary, independent relationship between independent features and acceptance.  In testing for discrimination, the project utilized a stepwise framework comparing a model built strictly on legitimate financial factors (68.6% accuracy) against one that included protected applicant demographics (68.8% accuracy). The marginal 0.2% difference ultimately supports the conclusion that, on an aggregate level, demographic traits 

<img width="500" alt="model-comparison-plot" src="https://github.com/user-attachments/assets/3175b878-ed64-4ff3-9773-eceeebf5a547" />

## [Predicting the Poverty Probability Index](https://github.com/justin-sharber/PPI)
Attempts to predict the Poverty Probability Index (PPI) from survey data.  The top performing model was found to be linear regression, with a very limited goodness-of-fit score of R-squared = 0.359.  The poor predictive performance of the models is investigated, and numerous issues are found in the data, with the only true numeric features having no correlation on the target variable.  Feature importances are evaluated with some surprising results: while geographic country, education level, and religion are significant features in the predictive model, certain mathematical skills and technology access have little to no impact.  

<img width="400" alt="linear-regression-correlation" src="https://github.com/user-attachments/assets/1743ddca-8838-4bc8-8c30-009aaf19f55a" />
