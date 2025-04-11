# ML-CatPrep: Flexible Machine Learning Framework for Data Preprocessing

## Overview
ML-CatPrep is a comprehensive algorithm and framework designed to handle missing values in categorical data using any machine learning technique. Traditional methods for handling missing values often lead to information loss or introduce bias, which negatively impacts downstream model performance. This project provides a flexible architecture that can leverage any ML algorithm to intelligently impute missing categorical values, resulting in significantly improved prediction accuracy compared to conventional preprocessing approaches. While currently focused on categorical data, the framework is designed to be expanded to handle numeric data in future releases.

Our experiments show that datasets preprocessed with ML-CatPrep lead to significantly higher predictive performance in downstream machine learning tasks compared to traditional imputation methods.

## Performance Metrics
The following table shows the performance comparison between different algorithms when used for target prediction after preprocessing with our framework:

| Metric | KNN | DT | NB |
|--------|-----|----|----|
| Accuracy | 0.982072 | 0.994313 | 0.841548 |
| Recall | 0.982072 | 0.994313 | 0.841548 |
| Precision | 0.982072 | 0.994313 | 0.841548 |
| F1 Score | 0.982072 | 0.994313 | 0.841548 |

As shown above, preprocessing with our framework significantly improves downstream machine learning performance. When using the Decision Tree (DT) approach for preprocessing, subsequent models achieve an impressive 99.43% accuracy, followed by K-Nearest Neighbors (KNN) preprocessing at 98.21%, while Naive Bayes (NB) preprocessing achieves 84.15%. These metrics demonstrate how our preprocessing approach leads to better predictive performance compared to traditional methods.

## Key Features
- **Flexible Algorithm Framework**: Designed to work with any machine learning algorithm, not limited to the provided implementations
- **Intelligent Missing Value Imputation**: Uses machine learning to predict and fill missing categorical values
- **Extensible Architecture**: Currently focused on categorical data with planned expansion to numeric data
- **Multiple Algorithm Implementations**: Includes ready-to-use implementations for KNN, Decision Trees, and Naive Bayes
- **High Accuracy**: Achieves up to 99.43% accuracy with the current implementations
- **Easy Integration**: Simple API that accepts datasets and returns fully preprocessed data
- **Minimal Data Loss**: Preserves data integrity better than traditional preprocessing methods
