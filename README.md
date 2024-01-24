# README

## Project Overview

This project analyzes a dataset from ProPublica to predict recidivism risk. The dataset includes 7,214 individuals and their characteristics like age, sex, race, and recidivism status. We performed data preprocessing, feature engineering, selection, cleaning, imbalance handling, and scaling. Various models, including linear and non linear classifiers, ensembles, and boosting algorithms, were tested. The highest accuracy of 69.37% was achieved with a gradient boosting machine. False positive rates were computed for African-American and Caucasian individuals, revealing bias towards the former. We also explored bias mitigation using a Diversity Parity fair classifier. These biases have societal implications, perpetuating systemic racism and discrimination

## Problem Statement

The central question revolves around the fairness of the predictive model in the context of criminal justice decision-making. Specifically, the project aims to address two key questions:

1. **Bias in terms of opportunity cost:** Examining false positive rates for African-American and Caucasian individuals to identify potential bias and its societal implications.

2. **Bias in terms of calibration:** Assessing calibration by comparing recidivism probabilities for African-American and Caucasian individuals predicted as positive by the algorithm.

## Report Summary

The provided report follows a structured approach, covering the following key sections:

1. **Introduction:** Setting the context for the COMPAS algorithm and the concerns related to bias in criminal justice predictions.

2. **Methodology:** Detailing the data visualization, preprocessing steps, and model training techniques used in the analysis.

3. **Identifying Bias:** Discussing the calculated false positive rates and recidivism probabilities, highlighting the observed bias towards African-American individuals.

4. **Impact of Race Variable:** Analyzing the impact of removing the race variable on the model's accuracy and biases.

5. **Using a Fair Classifier:** Exploring the use of a fair classifier to mitigate bias, with an emphasis on the trade-off between fairness and accuracy.

6. **Conclusion:** Summarizing the key findings and emphasizing the importance of ethical machine learning practices.

## Insights and Recommendations

The analysis reveals notable bias towards African-American individuals in the COMPAS algorithm, raising concerns about systemic racism and discrimination. The impact of removing the race variable suggests the presence of indirect correlations, emphasizing the need for careful consideration of protected features. The use of a fair classifier shows promise in improving fairness but highlights the trade-off between fairness and accuracy.

## Future Directions

The project underscores the importance of ongoing research and development in creating inclusive and equitable AI systems. Future work could explore more advanced fairness metrics, address potential indirect correlations, and delve into specific domains where different fairness measures may be more appropriate.

**File Structure:**
- data/compas-scores-two-years.csv
- auditing_for_bias_code.ipynb
- auditing_for_bias_report.pdf
- requirements.txt

**Note:** This README provides a concise overview of the project, and readers are encouraged to refer to the full report for detailed insights and analysis.

The ProPublica's story can be read here and their analysis can be found here. The COMPASS' defence can be read here. 

## Declaration
Project submitted towards the partial procurement of credits for CS584 Introduction to Data Mining at GMU under Professor Sanmay Das.