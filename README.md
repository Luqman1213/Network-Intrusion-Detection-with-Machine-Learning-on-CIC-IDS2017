# Network Intrusion Detection with Machine Learning on CIC-IDS2017

Overview

This repository contains the implementation and experimental evaluation of machine learning–based intrusion detection techniques using the CIC-IDS2017 dataset. The project investigates the effectiveness of supervised learning models for binary network intrusion detection under controlled experimental conditions. Two classification algorithms are evaluated: Logistic Regression and Random Forest. The study focuses on data preprocessing, feature analysis, model training, and performance evaluation using standard classification metrics.

Dataset

The experiments are conducted using the CIC-IDS2017 dataset, developed by the Canadian Institute for Cybersecurity (CIC). The dataset simulates realistic enterprise network traffic and includes both benign and malicious network flows across multiple attack scenarios. Due to size and licensing considerations, the dataset is not included in this repository. The dataset can be obtained from the official source: https://www.unb.ca/cic/datasets/ids-2017.html. Users must download the dataset separately and specify the local path in the notebook.

Methodology

The experimental workflow consists of data selection and sampling to reduce computational overhead while preserving class distribution, data preprocessing including feature removal, normalization, outlier handling, and binary encoding of labels, feature analysis through correlation and variance inspection, model training using Logistic Regression and Random Forest classifiers, and evaluation using confusion matrices, ROC curves, AUC scores, precision–recall curves, and standard classification metrics such as accuracy, precision, recall, and F1-score.

Results Summary

Logistic Regression achieved strong performance with high interpretability and an AUC close to 1.0, while Random Forest consistently outperformed Logistic Regression and achieved perfect classification performance on the evaluated subset. The results demonstrate the advantage of ensemble methods in capturing complex, non-linear patterns in network traffic.

Repository Structure

The repository contains a Jupyter notebook implementing the full experimental workflow, a README file documenting the project, an MIT license file, and a gitignore file specifying excluded files.

How to Run

To reproduce the results, download the CIC-IDS2017 dataset from the official source, update the dataset path in the notebook to point to the local dataset directory, and execute the notebook sequentially.

Requirements

The project was implemented using Python 3.12 with common scientific libraries including NumPy, Pandas, Scikit-learn, and Matplotlib.

License

This project is licensed under the MIT License.

Author

Muhammad Luqman, MSc Computer Science, University of Basel.
