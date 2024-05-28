# Linear Regression for Predicting Hiring

## Overview
This repository contains code for a simple linear regression model to predict hiring based on historical data. The model is built using Python and the scikit-learn library.

## Dataset
The dataset used for training the model is included in the repository as `hiring.csv`. It contains the following columns:
- `experience`: Years of experience of the candidate.
- `test_score(out of 10)`: Test score achieved by the candidate (out of 10).
- `interview_score(out of 10)`: Interview score achieved by the candidate (out of 10).
- `salary($)`: Salary offered to the candidate in dollars.

## Dependencies
To run the code in this repository, you'll need the following dependencies:
- math
- word2number
- pandas
- scikit-learn

You can install the dependencies using pip.

## Result
The formula is y = a1 * x1 + a2 * x2 + a3 * x3 + b for our data. x1, x2, x3 are features. a1, a2, a3 represent the coefficient or slope of the line which I found it with "reg.coef_" code. b represents the y-intercept which I found it with "reg.intercept_" code:
- a1 = 2812.95487627
- a2 = 1845.70596798
- a3 = 2205.24017467
- b = 17737.263464337688
- If we want to find the salary for 2 years experience, 9.0 test score, 6 interview score, our x1, x2, x3 will be 2, 9.0, 6.
- y = 2812.95487627 * 2 + 1845.70596798 * 9.0 + 2205.24017467 * 6 + 17737.263464337688 and y will be 53205.96797671 as in the given example.
