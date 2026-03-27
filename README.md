# StudentPerformanceAnalysis

## Project Overview
This project implements a **Linear Regression** model from scratch to predict student performance indices based on several academic and lifestyle factors. It was developed as part of "Đồ án 3" (Project 3) for a  machine learning course.

## Features
The model uses the following features to predict the **Performance Index**:
* **Hours Studied**: Total number of hours spent studying.
* **Previous Scores**: Scores obtained in previous exams.
* **Extracurricular Activities**: Participation in extracurricular activities (binary).
* **Sleep Hours**: Average hours of sleep per day.
* **Sample Question Papers Practiced**: Number of sample papers completed.

## Implementation Details
The project includes:
* **Data Exploration**: Statistical analysis and visualization of the student dataset.
* **Manual Model Implementation**: Linear Regression calculated using the normal equation and Moore-Penrose inverse (`np.linalg.pinv`) rather than relying solely on high-level libraries for the core algorithm.
* **Validation**: Implementation of K-Fold Cross-Validation to ensure model robustness.
* **Evaluation**: Performance is measured using **Mean Absolute Error (MAE)**.

## Model Performance
The best model achieved a **Mean Absolute Error (MAE)** of approximately **1.595** on the test dataset.

### Final Regression Equation
The derived relationship for predicting performance is:
$$\text{Performance Index} = -33.774 + 2.852 \times \text{Hours} + 1.018 \times \text{Prev. Scores} + 0.603 \times \text{Extracurricular} + \dots$$

## Requirements
To run this notebook, you need the following Python libraries:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`

## How to Use
1.  Ensure `train.csv` and `test.csv` are in the project directory.
2.  Open `solution.ipynb` in a Jupyter environment.
3.  Run all cells to perform data analysis, train the model, and view the evaluation results.
