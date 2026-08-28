# House Prices - Advanced Regression Techniques

This is my second Machine Learning project.

I participated in the Kaggle competition: **House Prices - Advanced Regression Techniques**.

### Competition Link

https://www.kaggle.com/competitions/home-data-for-ml-course

---

### Project Overview

The goal of this project is to predict the **sale price of houses** based on features describing different aspects of the properties.

The dataset contains information about things such as:

* Lot area
* Overall quality
* Number of rooms
* Year built
* Garage information
* Basement information
* Neighborhood
* And many other property features

The target variable is `SalePrice`.

---

### What I Did

1. Loaded and explored the housing dataset
2. Inspected the dataset shape, data types, and missing values
3. Removed columns with large amounts of missing data
4. Investigated the remaining missing values
5. Handled missing data
6. Prepared the features and target variable
7. Created a train-test split
8. Trained multiple regression models
9. Evaluated the models using **Root Mean Squared Error (RMSE)**
10. Compared the models
11. Used the best-performing model to predict house prices in the Kaggle test dataset
12. Created and submitted the `submission.csv` file to Kaggle

---

### Models Used

I tested several regression models:

* Linear Regression
* Ridge Regression
* Linear SVR
* Random Forest Regression

The models were compared using RMSE.

**Lower RMSE = better performance.**

| Model                    | Result                       |
| ------------------------ | ---------------------------- |
| Linear Regression        | ~46,754 RMSE                 |
| Ridge Regression         | Lower than Linear Regression |
| Linear SVR               | ~52,386 RMSE                 |
| Random Forest Regression | **~29,403 RMSE**             |

### Final Model

**Random Forest Regression** performed the best among the models I tested on my validation data.

The final Random Forest model was then used to generate predictions for the Kaggle test dataset.

---

### Kaggle Result

**Public Kaggle Score: 17,619.11528**

The Kaggle score is based on the competition's hidden test data, so it is different from the RMSE calculated on my local validation set.

---

### How to Run

1. Open the notebook in Google Colab or Jupyter
2. Make sure `train.csv` and `test.csv` are available
3. Run the notebook cells in order
4. Train the models
5. Compare their RMSE scores
6. Generate predictions using the final model
7. The `submission.csv` file will be generated

---

### Files

* `housing_prices_competition.ipynb` → Main Machine Learning notebook
* `train.csv` → Training dataset
* `test.csv` → Test dataset
* `data_description.txt` → Description of the dataset features
* `sample_submission.csv` → Example submission format
* `submission.csv` → Final predictions submitted to Kaggle

---

### Learnings

Through this project I learned:

* How to work with a larger real-world dataset
* How to inspect and handle missing values
* Why preprocessing is important before training a model
* How to split data into training and testing sets
* How regression models are used to predict continuous values
* How `random_state` helps make experiments reproducible
* How to use RMSE to evaluate regression models
* How to compare multiple Machine Learning models
* How to generate predictions for unseen data
* How to create a Kaggle submission

---

### Author

Akhilesh
