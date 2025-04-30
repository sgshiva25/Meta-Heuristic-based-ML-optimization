Here’s the updated README content with the **Methodology** section included:

---

# PET Bottle Defect and Component Classification: Metaheuristic Optimization Algorithms

This repository contains Python implementations of metaheuristic optimization algorithms used for feature selection in the hybrid approach for classifying PET bottle defects and components. These implementations are designed to work with machine learning classifiers to enhance the accuracy of defect detection and component classification.

## Files in This Repository

1. **`BBA.ipynb`**: Implementation of the Binary Bat Algorithm for feature selection.
2. **`EO.ipynb`**: Implementation of the Equilibrium Optimizer for feature selection.

---

## Table of Contents
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

The files in this repository demonstrate the use of metaheuristic optimization algorithms for selecting the most relevant features in PET bottle defect and component classification. These algorithms play a crucial role in reducing feature space dimensionality and improving the accuracy of machine learning classifiers.

---

## Methodology

The classification process follows a systematic workflow to optimize and classify features effectively. The steps include:

1. **Data Preprocessing**:
   - Input images are preprocessed to remove noise and enhance important features.

2. **Feature Extraction**:
   - Texture features like Contrast, Dissimilarity, Homogeneity, Energy, and Correlation are extracted using the Gray-Level Co-occurrence Matrix (GLCM).
   - Additional features such as Area, Perimeter, and Color Channel Statistics (Mean and Standard Deviation) are calculated.

3. **Feature Optimization**:
   - Metaheuristic algorithms (e.g., Binary Bat Algorithm and Equilibrium Optimizer) are used to reduce the feature set to the most relevant features for classification.
   - These algorithms balance exploration and exploitation to identify optimal feature subsets.

4. **Classification**:
   - Optimized features are passed to machine learning classifiers like Random Forest, SVM, and KNN.
   - Classifiers are trained on balanced datasets (addressing class imbalance using SMOTE).

5. **Evaluation**:
   - The performance of each classifier is evaluated using metrics like Accuracy, Precision, Recall, and F1-Score.
   - The combination of the Equilibrium Optimizer and Random Forest achieved the best results in this study.

---

## Features

- **Binary Bat Algorithm (`BBA.ipynb`)**:
  - Mimics the echolocation behavior of bats.
  - Balances exploration and exploitation to identify optimal feature subsets.

- **Equilibrium Optimizer (`EO.ipynb`)**:
  - Inspired by dynamic and equilibrium states in control systems.
  - Efficiently identifies high-quality feature subsets for improved classification.

---

## Prerequisites

To run these notebooks, ensure you have the following installed:
- Python 3.7 or higher
- Jupyter Notebook
- Required libraries:
  - NumPy
  - Pandas
  - Scikit-learn
  - Matplotlib


---

## Usage

### Running the Notebooks

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/pet-bottle-metaheuristics.git
   cd pet-bottle-metaheuristics
   ```

2. Open the desired notebook:
   ```bash
   jupyter notebook BBA.ipynb
   ```
   or
   ```bash
   jupyter notebook EO.ipynb
   ```

3. Follow the instructions in the notebook to:
   - Load the dataset.
   - Apply the respective optimization algorithm.
   - Analyze the selected features.

4. Use the optimized features with machine learning classifiers for classification tasks.

---

## Results

### Performance Metrics:
The optimized features selected by these algorithms can improve the accuracy, precision, and recall of machine learning classifiers. For instance:
- **Equilibrium Optimizer + Random Forest** achieved an accuracy of **88.26%** in PET bottle defect and component classification.

For a detailed breakdown of results, refer to the results section in the notebooks.

---

## Contributing

Contributions are welcome! Feel free to:
- Submit issues for bugs or suggestions.
- Create pull requests with your enhancements.

