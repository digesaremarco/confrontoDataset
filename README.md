# Notebook that compares CICids2017 and CICIoT2023

## Overview

This Jupyter notebook aims to compare and balance two network traffic datasets: Cicids2017 and Ciciot2023. The goal is
to analyze the class distribution within each dataset and ensure that the classes are balanced for downstream tasks such
as machine learning or statistical analysis.

## Datasets

1. Cicids2017: This dataset contains network traffic data and is commonly used for intrusion detection research. It
   includes various classes such as DoS attacks, web attacks, and benign traffic.

2. Ciciot2023: Another network traffic dataset used for similar purposes, containing a wide range of classes including
   DDoS
   attacks, reconnaissance activities, and benign traffic

## Notebook Contents

### Cicids2017 Dataset

- Data Loading: The notebook starts by loading the Cicids2017 dataset from disk, handling missing values and infinity
  values.
- Data Exploration: It explores the dataset by printing the first 5 rows, shape, and columns of the dataframe.
- Class Distribution: It visualizes the class distribution in the dataset using a histogram.
- Balancing: The dataset is balanced by downsampling the majority class to match the size of the minority class,
  ensuring balanced representation of classes.
- Histogram After Balancing: A histogram is plotted again to visualize the balanced class distribution.

### Ciciot2023 Dataset

- Data Loading: Similar to Cicids2017, this section loads the Ciciot2023 dataset from disk and handles missing values
  and infinity values.
- Data Exploration: Prints the first 5 rows, shape, and columns of the Ciciot2023 dataframe.
- Class Distribution: Visualizes the class distribution in the dataset using a histogram.
- Balancing: Due to an imbalance in the dataset, a more complex balancing strategy is employed. Majority classes are
  downsampled to match the size of the minority classes.
- Histogram After Balancing: A histogram is plotted again to visualize the balanced class distribution after applying
  the balancing strategy.

## Conclusion

Conclusion
This notebook provides a step-by-step guide to compare and balance network traffic datasets Cicids2017 and Ciciot2023,
ensuring a more equitable representation of classes for subsequent analysis tasks.

## Future Work: Federated Learning for IoT Intrusion Detection Systems

Use the notebook to compare and evaluate the Cicids2017 and Ciciot2023 datasets for suitability in a federated learning
setting for IDS on IoT devices.
Factors to consider include class distribution, data size, and compatibility with federated learning algorithms.