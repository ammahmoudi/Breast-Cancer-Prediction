# Breast-Cancer-Prediction

An exploratory data analysis (EDA) and machine learning on the "Breast Cancer Gene Expression Profiles (METABRIC)" dataset.
The primary goal is to gain insights and understanding from the dataset, especially regarding clinical information and its relationship with breast cancer survival.


## Data Documentation
We will use "Breast Cancer Gene Expression Profiles (METABRIC)" data.
- **Clinical Data**: The first 31 columns contain clinical information, including patient demographics, treatment details, and overall survival status.
- **Gene Expression Data**: These columns include gene expression values and provide insights into the genetic characteristics of patients.
- **Gene Mutation Data**: These columns contain information about gene mutations, which can be critical in cancer research. Gene's mutation info columns have been marked with \"\\_mut\" at the end of the names of the columns.
  
For more information please read the [data documentation](https://www.kaggle.com/datasets/raghadalharbi/breast-cancer-gene-expression-profiles-metabric).


## Code Explanation
In this project, the following tasks were performed:

1. **Data Loading**: I load the dataset from a CSV file and explore the initial records to understand its structure.

2. **Data Preparation**:
   - I split the data into three separate datasets: clinical, gene expression, and gene mutation. Each dataset includes the `patient_id` and `overall_survival` columns for future analysis.
   - Data type warnings are addressed to ensure data consistency.

3. **Exploratory Data Analysis (EDA)**:
   - I conducted an EDA on the clinical data, including:
     - Identifying missing values and visualizing their percentages.
     - Creating box plots to explore the distribution of numerical attributes.
     - Plotting histograms for key clinical variables based on overall survival status to uncover potential patterns.

4. **Data Transformation**:
   - I created dummy variables for categorical columns in the clinical data, making them suitable for modeling.
5. **Dimension Reduction**:
   - Trying to reduce dataset dimension using UMAP, PCA, Autoencoder
6. **Model training and Results**:
   - predict breast cancer using several machine-learning classification models.
   - Baseline models including Logistic Regression, SVM, Naive Bayes, and Random Forest are implemented using Scikit-Learn.
   - The models are evaluated and compared using accuracy, precision, recall, and ROC AUC metrics.
   - Key techniques employed include data preprocessing, hyperparameter tuning using GridSearchCV, and cross-validation to combat overfitting.
   - Visualizations including correlation plots and confusion matrices provide additional insight into model performance.

The XG_BOOST classifier achieved the best performance.
This end-to-end implementation serves as a guide for applying core machine learning concepts to classify and predict breast cancer from medical imaging data. There may be some issues and problems in data and models which are skipped.
![result](/output.png)

Please refer to the code file for a detailed explanation and code implementation.

