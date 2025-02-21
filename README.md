# Titanic Dataset Project

## 1. Dataset Story
The Titanic dataset contains information about the passengers aboard the RMS Titanic, which sank on April 15, 1912. This dataset is commonly used in data science projects to predict survival outcomes. The ship carried 2,224 passengers, and approximately 68% of them lost their lives.

## 2. Dataset Structure
- **Number of Observations (Rows):** 891
- **Number of Variables:** 11
- **Variable Types:**
  - `Survived` (category)
  - `Pclass` (int64)
  - `Name` (category)
  - `Sex` (category)
  - `Age` (float64)
  - `SibSp` (int64)
  - `Parch` (int64)
  - `Ticket` (category)
  - `Fare` (float64)
  - `Cabin` (category)
  - `Embarked` (category)

### Missing Data Status
- `Age`: 177 missing values
- `Cabin`: 687 missing values
- `Embarked`: 2 missing values

## 3. Data Visualization Methods
Methods used:
- **Bar Plot**
- **KDE Plot (Kernel Density Estimation)**
- **Box Plot**

## 4. Outlier and Missing Data Issues
### Outlier Detection
- **IQR method** was used to identify outliers.
- Outliers in `Fare` were capped at an upper threshold.
- Outliers in `Age` (above 80 years) were replaced with the median age.

### Missing Data Solutions
- `Age`: Filled using median values grouped by `Pclass` and `Sex`.
- `Cabin`: Removed due to excessive missing values.
- `Embarked`: Filled with the most frequent value, "S".

## 5. Problem Type
The Titanic dataset is a **binary classification** problem. The target variable, `Survived`, has two possible values: 0 (Did not survive) or 1 (Survived).

## 6. Machine Learning Models Used
- **CART (Decision Tree)**
- **SVM (Support Vector Machine)**
- **Random Forest**
- **Gradient Boosting**

## 7. Model Performance Evaluation Metrics
- **Accuracy**
- **Average Precision**
- **Average F1-Score**
- **Recall**

## 8. Comparison of Machine Learning Results
Different models were compared based on accuracy and other evaluation metrics to determine the best-performing model.

## 9. Dimensionality Reduction Method
**Principal Component Analysis (PCA)** was used in this project to reduce the dataset's dimensionality while retaining most of the variance, optimizing model performance.

## 10. Model Performance Comparison
The best-performing model was evaluated on both the original dataset and the PCA-transformed dataset to compare their predictive performance.

