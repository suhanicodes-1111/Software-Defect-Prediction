# Software Defect Prediction Using Machine Learning (DA2)

**Course:** Programming for Data Science (PDS)
**Stage:** DA2 - Model Development, Database Connectivity & Comparative Analysis
**Dataset:** JM1 Software Defect Dataset (NASA PROMISE repository), 10,885 modules x 22 columns
**Tools:** R (RStudio), MySQL

## Run order
1. Download `jm1.csv` from the NASA PROMISE repository into the project folder.
2. `scripts/01_setup_data.R` - import and clean the data
3. `scripts/02_mysql_setup.sql` - create the MySQL database (run in MySQL Workbench)
4. `scripts/03_mysql_connectivity.R` - write to / read from MySQL (edit your username and password)
5. `scripts/04_feature_engineering.R` - engineered features, correlation filter, Boruta
6. `scripts/05_model_training.R` - trains and tunes the models in parallel
7. `scripts/06_evaluation_visualization.R` - metrics table, ROC, PR curves, confusion matrices, feature importance

`scripts/check_na.R` is a small diagnostic for missing values before training.

## Notes
- The dataset and `.rds` files are not committed (see `.gitignore`); the scripts regenerate them.
- Never commit your MySQL password.
- The written report is in `docs/DA2_Report.docx`.
