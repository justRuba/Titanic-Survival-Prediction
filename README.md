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

## Explore the data
- Number of rows and columns And Information about data:
   
![WhatsApp Image 2024-08-01 at 01 08 05_0b9e88e1](https://github.com/user-attachments/assets/70b284ea-e34f-404a-842b-2d3adfaf6c75)

- Show missing values in each column:
  
![WhatsApp Image 2024-08-01 at 01 09 03_4ba502b2](https://github.com/user-attachments/assets/9e899c42-0f99-4665-a61b-dfd3055eeed4)

- describe() provides summary statistics for numerical columns, including count, mean, standard deviation, min, max, and quartiles. corr() Calculates correlation coefficients (-1 to 1) to identify the strength and direction of linear relationships between features and survival in the Titanic dataset.

![WhatsApp Image 2024-08-01 at 01 19 26_888196d4](https://github.com/user-attachments/assets/20f2616a-d434-4829-9d08-73942400e6c5)

![WhatsApp Image 2024-08-01 at 01 27 51_8fb8a4ba](https://github.com/user-attachments/assets/222a02ae-fb48-4a47-adb2-a49d74654106)

- The plot shows the distribution of survival outcomes in the Titanic dataset. It displays the count of passengers who survived (Survived = 1) versus those who did not survive (Survived = 0).

![WhatsApp Image 2024-08-01 at 01 38 50_4d5f71d1](https://github.com/user-attachments/assets/7fcb8065-e8e3-499a-99ea-bb251eb7959d)

## Data Preprocessing

### Handle missing values

- Fill missing Age values with the mean age.

  ![WhatsApp Image 2024-08-01 at 01 50 21_b40cc6b0](https://github.com/user-attachments/assets/cbe521d6-4736-4692-be1c-171a1bc52dde)

- Drop the Cabin column due to a high percentage of missing values.

  ![WhatsApp Image 2024-08-01 at 01 51 46_96ae2ae2](https://github.com/user-attachments/assets/78744781-c127-424c-b580-0b129cd008d7)

- Fill missing Embarked values with the mode.

  ![WhatsApp Image 2024-08-01 at 01 56 48_4eb412a8](https://github.com/user-attachments/assets/355323f7-d9c2-46f8-af0a-d79ff8b90ef6)

### Drop unnecessary columns: PassengerId, Name, Ticket

![WhatsApp Image 2024-08-01 at 02 02 27_2d03f4ec](https://github.com/user-attachments/assets/95663bc9-965b-4a37-977d-05ee36c74e1b)

### Encode categorical columns: Sex, Embarked

![WhatsApp Image 2024-08-01 at 02 03 54_3e456cf7](https://github.com/user-attachments/assets/c2d1b2fd-5111-4983-86db-c61d11a1cf16)

### Handle duplicate rows

![WhatsApp Image 2024-08-01 at 02 05 02_4bb5abc5](https://github.com/user-attachments/assets/58cb5242-8198-4ac1-8092-6088e45cd0e9)


## Analysis of our data

- The plot shows the distribution of passengers by gender in the Titanic dataset. It displays the count of male and female passengers, illustrating the number of passengers in each gender category.

![WhatsApp Image 2024-08-01 at 01 40 52_f27f140f](https://github.com/user-attachments/assets/4838a31a-df76-40f0-b523-899f776cbc4b)

- The plot shows the distribution of passengers by gender, with survival outcomes indicated by color. It displays counts of male and female passengers who survived and did not survive, providing insight into survival rates across genders.

![WhatsApp Image 2024-08-01 at 01 43 47_bda89f4c](https://github.com/user-attachments/assets/dc7008d9-cb34-400f-98ac-85258b54c0e1)

- The plot shows the distribution of passengers across different classes (Pclass), with survival outcomes indicated by color. It illustrates the count of passengers in each class who survived versus those who did not, highlighting survival rates by class.

![WhatsApp Image 2024-08-01 at 01 45 09_378ec262](https://github.com/user-attachments/assets/dcf45d95-2060-46d3-abbd-09cb9f7aa616)
