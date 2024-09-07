# Cirrhosis Patient Survival Prediction

This repository contains the code and resources for building machine learning models to predict the survival status of patients with liver cirrhosis. The dataset used comes from the Mayo Clinic's study on primary biliary cirrhosis (PBC) of the liver conducted between 1974 and 1984. The objective of this project is to predict the survival status of cirrhosis patients based on clinical features.

## Dataset Information

- **Data Source**: [Cirrhosis Patient Survival Prediction Dataset](https://archive.ics.uci.edu/dataset/878/cirrhosis+patient+survival+prediction+dataset-1)
- **Number of patients**: 418
- **Number of features**: 17
- **Survival states**:
  - 0: D (Death)
  - 1: C (Censored)
  - 2: CL (Censored due to liver transplantation)

### Features

The dataset includes the following features:
1. ID
2. Age (in years)
3. Gender (M = Male, F = Female)
4. Days since registration
5. Status (0 = D, 1 = C, 2 = CL)
6. Drug
7. Ascites
8. Hepatomegaly
9. Spiders
10. Edema
11. Bilirubin
12. Cholesterol
13. Albumin
14. Copper
15. Alk_phosphate
16. SGOT
17. Triglycerides
18. Platelets
19. Prothrombin

## Project Structure

- **JakeTolentino_cirrhosis.ipynb**: Jupyter notebook containing the code for data exploration, preprocessing, model training, and evaluation.
- **Report.pdf**: A report detailing the steps taken and answers to specific questions provided in the task.

## Installation and Setup

1. Clone this repository:

    ```bash
    git clone <repository-url>
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Open the Jupyter notebook:

    ```bash
    jupyter notebook JakeTolentino_cirrhosis.ipynb
    ```

## Data Preprocessing

### 1. Handling Missing Values
The dataset contains missing values, which were handled using appropriate imputation techniques.

### 2. Train-Test Split
The data was split into an 80:20 ratio for training and testing purposes.

### 3. Feature Types
The features were classified as continuous or categorical, and necessary encoding was performed for the categorical features.

### 4. Label Distribution
The label distribution was analyzed to check for class imbalance. Methods to deal with label imbalance were implemented during the model training phase.

## Machine Learning Models

The following machine learning models were used for predicting the survival status:

1. **Logistic Regression**
2. **Random Forest**
3. **Support Vector Machine (SVM)**

### Model Evaluation
- Performance was evaluated using various metrics such as accuracy, precision, recall, and F1-score.
- Hyperparameter tuning was performed to optimize the models.
- Techniques such as cross-validation were used to ensure the model is not underfitted or overfitted.

### Imbalanced Dataset Handling
A method for handling label imbalance was applied, and its effect on model performance was evaluated.

### Feature Importance
Two different methods were used to analyze the importance of features in predicting the survival status.

## Results

- The results from all models were compared, and the best-performing model was selected based on its performance on the test set.
- The model performance and justification for selecting the best model are provided in the accompanying report.

## References

- **Dataset**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/878/cirrhosis+patient+survival+prediction+dataset-1)
- **Cirrhosis Background**: Mayo Clinic Study

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
