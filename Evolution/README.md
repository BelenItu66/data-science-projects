# Hominid Chronology and Classification
## Machine Learning Applications in Paleoanthropology
## Project Overview
One of the major challenges in paleoanthropology is accurately classifying and dating hominid fossils. Traditional methods, such as radiocarbon dating and isotope analysis, are often expensive, invasive, or require specific materials. This project explores how machine learning can be used to classify fossils by genus and species and estimate their geological age based on their physical traits.
## Objectives
- **Taxonomic Classification of Fossils**
  - Develop supervised classification models to predict the genus and species of hominid fossils using physical traits like cranial size, bone length, and endocranial capacity.
- **Chronological Estimation**
  - Build regression models to estimate the geological age of fossils based on physical characteristics.
## Dataset
The dataset used for this project is sourced from Kaggle, containing 12,000 fossil records with 27 attributes. It includes data on taxonomic classification, fossil characteristics, and estimated time periods.

**Dataset Link:**[Biological Data of Human Ancestors](https://www.kaggle.com/datasets/santiago123678/biological-data-of-human-ancestors-data-sets?select=Homininos_DataSet+%281%29.csv)
## Data Processing
### Data Cleaning
- No missing values required imputation.
- Standardized column names for better readability
- Transformed time variables into a numerical format (millions of years before present).
- Normalized cranial capacity values (expressed in cm³).

## Exploratory Data Analysis (EDA)
- Species distribution over time
- Geographical fossil distribution
- Correlation between cranial capacity and jaw shape
- Evolutionary trends in hominid brain size
## Machine Learning Models
### Classification Models (Genus & Species Prediction)
- Random Forest Classifier
- Multilayer Perceptron (MLP)
- Gradient Boosting Classifier
**Hyperparameter Optimization:** RandomSearchCV
**Evaluation Metrics:** Precision, Recall, R²
### Regression Models (Fossil Age Estimation)
- Random Forest Regressor
- MLP Regressor
**Hyperparameter Optimization:** GridSearchCV
**Evaluation Metrics:** R², MAE
## Key Findings
- Taxonomic classification models achieved high accuracy, confirming that hominid traits follow consistent patterns useful for classification.
- Geological dating models provided reliable time estimates, serving as a complementary tool when absolute dating is not available.
- Random Forest performed best for taxonomic classification, while MLP excelled in predicting fossil age.
## Future Work 
- Expand dataset with additional fossil samples and new regional data.
- Develop a reproducible framework for applying machine learning to forensic anthropology.
- Improve classification models by incorporating new anatomical features.

