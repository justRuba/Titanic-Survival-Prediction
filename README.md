# Titanic-Survival-Prediction

This project involves analyzing the Titanic dataset to predict the survival of passengers using a Logistic Regression model. The project includes data preprocessing, feature engineering, model building, evaluation, and visualization.

## Introduction

The Titanic dataset provides information on the passengers who were aboard the Titanic. This project aims to build a predictive model that can determine whether a passenger survived or not based on features such as age, sex, class, and fare.

## Dataset

The dataset used in this project is the Titanic dataset, which can be found on [Kaggle](https://www.kaggle.com/competitions/titanic/data). The dataset includes the following columns:

![WhatsApp Image 2024-08-01 at 01 01 46_96e8de1e](https://github.com/user-attachments/assets/2d007554-b5ea-4b3c-a411-42be8a7ba4a2)

- `PassengerId`: Passenger identifier
- `Survived`: Survival indicator (0 = No, 1 = Yes)
- `Pclass`: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Passenger name
- `Sex`: Passenger sex
- `Age`: Passenger age
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Ticket`: Ticket number
- `Fare`: Fare paid
- `Cabin`: Cabin number
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Dependencies

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

## Explore and analysis the data
- Number of rows and columns And Information about data:
   
![WhatsApp Image 2024-08-01 at 01 08 05_0b9e88e1](https://github.com/user-attachments/assets/70b284ea-e34f-404a-842b-2d3adfaf6c75)

- Show missing values in each column:
  
![WhatsApp Image 2024-08-01 at 01 09 03_4ba502b2](https://github.com/user-attachments/assets/9e899c42-0f99-4665-a61b-dfd3055eeed4)

- describe() provides summary statistics for numerical columns, including count, mean, standard deviation, min, max, and quartiles. corr() Calculates correlation coefficients (-1 to 1) to identify the strength and direction of linear relationships between features and survival in the Titanic dataset.

![WhatsApp Image 2024-08-01 at 01 19 26_888196d4](https://github.com/user-attachments/assets/20f2616a-d434-4829-9d08-73942400e6c5)

![WhatsApp Image 2024-08-01 at 01 27 51_8fb8a4ba](https://github.com/user-attachments/assets/222a02ae-fb48-4a47-adb2-a49d74654106)


## Data Preprocessing

