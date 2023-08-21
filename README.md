# data_analysis_synthetic_edu_data

## Table of Contents

- [Project Description](#project-description)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Results and Discussion](#results-and-discussion)
- [Fairness Evaluation](#fairness-evaluation)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Project Description

This project presents an analysis of a fictional educational dataset including the following data: ID, Gender, Race, Grade, Attendance Rate, Free or Reduced Lunch, Primary Language, Lives with Parent/Guardian, Promoted, SEL Score, Reading Level, Case Managed, and Average Grade. While the data isn't real, and there could be many more variables to factor into a real predictive model for student-level education outcomes, this project is being used with the goal of creating a basic predictive model to determine which of the included variables are significant in predicting if a given student was promoted or retained. This dataset consists of 657 observations across 14 columns/variables and includes both continuous and categorical variables.

## Installation and Setup

To run this notebook, you will need to have Python 3 installed along with the following libraries: pandas, numpy, matplotlib, seaborn, and scikit-learn. You can install these libraries using pip: pip install pandas numpy matplotlib seaborn scikit-learn


Once you have installed the required libraries, you can open the notebook in Jupyter and run each cell in order.

## Usage

This notebook is designed to be used as a guide for analyzing a similar educational dataset and creating a decision tree model to predict student promotion. You can use this notebook as a starting point for your own analysis by replacing the fictional dataset with your own data and modifying the code as needed.

## Results and Discussion

After analyzing the dataset and creating a decision tree model using scikit-learn, we found that the following variables were the most important in predicting student promotion: whether a student was case managed, their attendance rate, whether or not they were at-risk of dropping out, and identifying as male. These variables could be helpful moving forward in identifying students who are at risk of not being promoted to the next grade.

## Fairness Evaluation

A fairness evaluation of the model was started using two metrics: equalized odds difference and impact ratio. The equalized odds difference measures the difference in true positive rates and false positive rates between the protected group (in this case, female students) and the unprotected group (male students). The impact ratio measures the ratio of the false positive rate of the protected group to the false positive rate of the unprotected group. Our analysis showed that the model had a higher false positive rate for female students than male students, indicating potential gender bias in the model.

## Future Work

While this notebook provides a basic framework for analyzing an educational dataset and creating a decision tree model, there are many ways to improve upon this work. Some possible avenues for future work include:

- Incorporating additional variables into the model
- Using more advanced machine learning techniques such as random forests or neural networks
- Collecting more observations to improve the accuracy of the model
- Further exploring and addressing potential biases in the model through additional fairness evaluations and adjustments to the model

## Contributing

If you would like to contribute to this project, please open an issue or pull request on GitHub.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
