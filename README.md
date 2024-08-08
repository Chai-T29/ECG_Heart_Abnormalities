# Welcome to the ECG 5000 Project!

### Project Overview

Hello, fellow Data Scientists! Are you ready to delve into the world of ECG data and predictive modeling? This project focuses on dimensionality reduction techniques for continuous functions, particularly for ECG data. Our goal is to detect heart signal variations, a crucial task for early detection of heart diseases.

We will cover various methodologies for transforming ECG data into machine-readable formats, making it suitable for classification tasks. This was an assignment  from [Professor Kamran Paynabar’s High-Dimensional Data Analytics class](#references) at Georgia Institute of Technology, so all credits go to his lectures. I've expanded on his assignment for multiclass modeling of ECG data to understand how this approach can be translated for variations of heart signals (rather than binary outputs). I gained a lot of knowledge from this material, and wanted to showcase it to you all as well!

### Key Objectives

1. How can we effectively reduce the dimensionality of ECG data?
2. How do different classification models perform on ECG data?
3. What insights can we gain about heart signals from our models?

### Project Components

The methodology and steps below are from [Professor Kamran Paynabar's High-Dimensional Data Analytics class](#references).

1. Setup: Importing Libraries and Loading Data: Getting all the necessary tools and data ready.
2. Exploratory Data Visualization: Understanding the data through visual analysis.
3. Preprocessing the Data: Preparing the data for modeling.
4. Basis Spline (B-Spline) Approach: Using B-Splines for dimensionality reduction.
5. Finding Optimal Number of Knots: Determining the best number of knots for B-Splines.
6. Fitting Model with Optimal Knots: Training a model with the optimal B-Spline configuration.
7. Functional Principal Component Analysis (FPCA): Alternatively using FPCA to reduce dimensionality.
8. Observations / Results: Analyzing the model performance and drawing insights.

### Data Description

The dataset includes:

- Training Data: 500 samples
- Testing Data: 4500 samples

Each sample has 140 features plus a target label (1 for normal and 0 for abnormal).

### Requirements

Before starting, ensure you have the following libraries installed:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn scikit-fda
```

### Workflow

1. Setup: Importing Libraries and Loading Data:
  - Import necessary libraries.
  - Load the ECG data from the source provided in the notebook.
  - Preprocess the data for analysis.
2. Exploratory Data Visualization:
  - Use visualizations to understand the structure and distribution of the data.
  - Identify any patterns or anomalies.
3. Preprocessing the Data:
  - Handle missing values.
  - Normalize the data for better model performance.
4. Basis Spline (B-Spline) Approach:
  - Use B-Splines to create a lower-dimensional representation of the ECG data.
  - Define the mathematical basis for B-Splines and their application.
5. Finding Optimal Number of Knots:
  - Determine the optimal number of knots for the B-Spline basis to achieve the best classification accuracy.
  - Visualize the accuracy scores for different numbers of knots.
6. Fitting Model with Optimal Knots:
  - Train a Support Vector Classifier (SVC) using the optimal B-Spline configuration.
  - Evaluate the model’s performance using various metrics.
7. Functional Principal Component Analysis (FPCA):
  - Apply FPCA to reduce the dimensionality of the data.
  - Compute the principal components and use them to train the model.
  - Assess the model’s performance.
8. Observations / Results:
  - Analyze the performance metrics of the models.
  - Compare B-Spline and FPCA approaches.
  - Discuss the implications for detecting heart abnormalities.

### Conclusion

By the end of this project, you will have a deep understanding of how to preprocess and reduce the dimensionality of ECG data, as well as how to apply various classification models to detect heart abnormalities. You’ll learn about B-Splines, FPCA, and their applications in high-dimensional data analytics. These skills are invaluable for developing effective models in medical diagnostics and other fields.

Happy learning!


### Disclaimer and Acknowledgments

This project is inspired by the teachings of [Professor Kamran Paynabar](#references) from his High-Dimensional Data Analytics class at Georgia Institute of Technology. The implementation in a multiclass setting, dataset used, and interpretation are my original work and not directly taken from the course materials.

### References

Paynabar, Kamran, "Intro to HD and Functional Data." Class lecture, High Dimensional Data Analytics, Georgia Institute of Technology, Atlanta, GA. May 13, 2024.
