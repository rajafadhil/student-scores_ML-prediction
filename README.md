# Predicting Student Scores Based on Study Hours

## Project Overview

This project uses machine learning regression models to predict student scores based on the number of hours they studied. We aim to determine which model performs best in predicting scores accurately. The dataset contains information on hours studied and corresponding scores, making it suitable for regression analysis.

## Files in This Repository

- **dataset.csv**: The dataset file containing two columns:
  - **Hours**: Number of hours studied by the student.
  - **Scores**: Score achieved by the student.
- **analysis.ipynb**: The Jupyter Notebook file where all analysis, model training, and evaluation steps are performed.
- **README.md**: This file, describing the project structure and objectives.

## Project Workflow

The workflow for this project includes the following steps, all documented in the `analysis.ipynb` notebook:

1. **Exploratory Data Analysis (EDA)**:
   - Loaded the dataset and explored it using descriptive statistics to understand data distribution.
   - Visualized the relationship between study hours and scores using scatter plots, histograms, and box plots.
   - Used a correlation heatmap to confirm the strong positive relationship between hours studied and scores.

2. **Data Preparation**:
   - Split the dataset into training and testing sets (80% training, 20% testing) to evaluate model performance on unseen data.

3. **Model Training**:
   - Trained three different regression models:
     - **Linear Regression**
     - **Decision Tree Regressor**
     - **Random Forest Regressor**
   - Each model was trained using the training set and then used to predict scores on the test set.

4. **Model Evaluation**:
   - Evaluated model performance using two key metrics:
     - **Mean Squared Error (MSE)**: Measures the average of the squared differences between predicted and actual values.
     - **R-squared (R²)**: Indicates how well the model explains the variance in the target variable (scores).
   - Based on these metrics, compared the three models to determine the most accurate one.

5. **Results**:
   - The results indicated that **Random Forest Regressor** performed best with the lowest MSE and the highest R-squared, making it the most accurate model for this dataset.

## Results Summary

| Model                   | Mean Squared Error | R-squared |
|-------------------------|--------------------|-----------|
| Linear Regression       | 18.94             | 0.97      |
| Decision Tree Regressor | 31.7              | 0.95      |
| Random Forest Regressor | 12.83             | 0.98      |

**Conclusion**: The **Random Forest Regressor** model achieved the highest accuracy, making it the best model for predicting student scores based on study hours in this dataset.

## How to Use This Project

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/yourprojectname.git
