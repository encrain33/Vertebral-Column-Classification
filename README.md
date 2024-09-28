# Vertebral Column Classification Project

This project demonstrates the application of unsupervised and supervised classification methods on a vertebral column dataset. It was completed as coursework for a Master's-level Advanced Statistics and Machine Learning course at the University of Manchester.

## Project Overview and Significance

The goal of this project was to classify orthopaedic patients as normal or abnormal based on biomechanical attributes of their vertebral column, using both unsupervised and supervised machine learning techniques. This project demonstrates the application of advanced statistical and machine learning methods to medical diagnostics, showcasing the potential for AI to assist in orthopedic patient classification.

The project was completed as coursework for a Master's-level Advanced Statistics and Machine Learning course, constrained to approximately 1000 words as per course requirements. It received full marks (20/20) in the course assessment, demonstrating proficiency in applying machine learning techniques to real-world problems.

## Important Note

This repository contains the project in its original form as submitted for coursework. No alterations or improvements have been made post-submission, providing an authentic view of the work completed within the course constraints.

## Dataset

The Vertebral Column Data Set from the UCI Machine Learning Repository, containing:
- 310 patients (210 abnormal, 100 normal)
- 6 biomechanical features and 1 class label

The dataset is stored in 'vertebral_column_data.txt'. The file does not contain column headers. The values in each row correspond to the following features in order:
1. pelvic_incidence
2. pelvic_tilt
3. lumbar_lordosis_angle
4. sacral_slope
5. pelvic_radius
6. grade_of_spondylolisthesis
7. class (AB: Abnormal, NO: Normal)

Note: The 'class' column is the target variable for classification.

## Methods Used

- Unsupervised Learning: K-means Clustering
- Supervised Learning: Support Vector Machine (SVM), Random Forest, K-Nearest Neighbours (KNN)
- Dimensionality Reduction: Principal Component Analysis (PCA)
- Data Transformation: Yeo-Johnson transformation for a skewed feature

## Key Findings

1. PCA revealed that the first two principal components explain 75.76% of the data variance.
2. K-means clustering showed limitations in separating the classes, likely due to non-spherical cluster shapes.
3. SVM performed best among supervised methods, achieving 90% accuracy on the validation set using all 6 PCs.
4. All supervised models performed better when using more than just the first two PCs, indicating the importance of the additional components.
5. The 'grade_of_spondylolisthesis' feature showed high discriminative power after transformation.

## File Structure and Contents

- `vertebral_column_analysis.ipynb`: Jupyter notebook containing the full analysis
- `vertebral_column_data.txt`: Dataset used for the analysis
- `vertebral_column_report.pdf`: Detailed project report including:
  - In-depth explanation of the methods used
  - Detailed analysis of results
  - Discussion of findings and their implications
  - Visualisations of key outcomes
- `README.md`: This file, providing project overview and instructions

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, scipy

## How to Run

1. Please ensure you have Jupyter Notebook or JupyterLab installed.
2. Install required libraries: `pip install pandas numpy scikit-learn matplotlib seaborn scipy`
3. Open `vertebral_column_analysis.ipynb` in Jupyter.
4. Run the cells in order to reproduce the analysis.

## Acknowledgements

This project was completed as part of an Advanced Statistics and Machine Learning course. Special thanks to the course instructor, Professor Lorenzo Pellis, for his feedback.
