# machine_learning_project-supervised-learning

## Project Outcomes
- Supervised Learning: use supervised learning techniques to build a machine learning model that can predict whether a patient has diabetes or not, based on certain diagnostic measurements.The project involves three main parts: exploratory data analysis, preprocessing and feature engineering, and training a machine learning model. 
### Duration:
Approximately 5 hours and 30 minutes.
### Project Description:
## Exploratory Data Analysis
Upon importing the dataset, an initial inspection of the data was performed using the `.info()` and `.describe()` methods, offering an overview of the dataset's structure and statistical summaries. Several essential checks were conducted, examining for null values, zeros, and missing data within the dataset. To delve deeper into the interrelationships between variables, a correlation heatmap was generated, providing insights into the pairwise correlations. Histograms were employed to visualize the distribution of the data, offering an understanding of the frequency distribution of the variables. Boxplots were created to identify and visualize outliers present in each column, providing insights into the spread and distribution of values. Furthermore, a comparative analysis was conducted by examining the data concerning diabetes status, allowing for a detailed comparison of the data distributions between the groups with and without diabetes. These comprehensive exploratory steps aimed to provide a thorough understanding of the dataset, its characteristics, and variations between groups, thereby laying the groundwork for further analysis and modeling.
## Feature Engineering
In the process of feature selection and data preprocessing, various techniques were employed. Initially, Variance Threshold and SelectKBest methods were applied to narrow down the feature set, opting for a reduced dimensionality. Subsequently, a train-test split was performed, allocating 80% of the data for training and 20% for testing. To handle missing values, zeros were replaced with NaN, following which the KNNImputer method was utilized to impute the missing data points. Outliers were detected using the Interquartile Range (IQR) method, and for the identified outliers, the median values of specific columns were used as replacements. Finally, StandardScaler was applied to standardize the data, ensuring that the values were on a similar scale before proceeding to modeling and analysis. This comprehensive preprocessing pipeline aimed to enhance the data quality and prepare it for effective model training and evaluation.
## Model building
The models constructed for this analysis involved the utilization of Logistic Regression and Random Forest Classifier. Subsequently, following a process of hyperparameter tuning facilitated by Gridsearch, it was evident that the Random Forest Classifier outperformed the Logistic Regression model in terms of accuracy. This optimization method allowed for the selection of the Random Forest Classifier as the more accurate and suitable model for the specific predictive task at hand.