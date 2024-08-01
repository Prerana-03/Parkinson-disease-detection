# Parkinson-disease-detection
# Parkinson's Disease Detection Using Logistic Regression

## Overview

This project implements a logistic regression model to diagnose Parkinson's disease using voice measurement data. The dataset is sourced from the [Oxford Parkinson's Disease Detection Dataset](https://archive.ics.uci.edu/dataset/174/parkinsons). The goal is to distinguish between healthy individuals and those with Parkinson's disease based on various vocal attributes.

## Dataset

The dataset consists of biomedical voice measurements from 31 individuals, including 23 diagnosed with Parkinson's disease (PD). Each row in the dataset corresponds to a voice recording, and the columns represent different voice measures. The primary target variable is "status," with 0 indicating healthy and 1 indicating PD.

- **Data Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/174/parkinsons)
- **Data Format**: CSV

### Features
- **name**: Subject name and recording number
- **MDVP:Fo(Hz)**: Average vocal fundamental frequency
- **MDVP:Fhi(Hz)**: Maximum vocal fundamental frequency
- **MDVP:Flo(Hz)**: Minimum vocal fundamental frequency
- **MDVP:Jitter(%), MDVP:Jitter(Abs), MDVP:RAP, MDVP:PPQ, Jitter:DDP**: Measures of variation in fundamental frequency
- **MDVP:Shimmer, MDVP:Shimmer(dB), Shimmer:APQ3, Shimmer:APQ5, MDVP:APQ, Shimmer:DDA**: Measures of variation in amplitude
- **NHR, HNR**: Ratios of noise to tonal components in the voice
- **status**: Health status of the subject (1 for Parkinson's, 0 for healthy)
- **RPDE, D2**: Nonlinear dynamical complexity measures
- **DFA**: Signal fractal scaling exponent
- **spread1, spread2, PPE**: Nonlinear measures of fundamental frequency variation

## Installation

To run this project, ensure you have the following Python packages installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

You can install the required packages using `pip`. Run the following command:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
