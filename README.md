# diabetic-retinopathy-is-referenceable-NPDR-Moderate-or-beyond-or-DPR-with-NDE-or-not.
Dataset
https://www.dropbox.com/sh/ik8hlcsieszypgq/AABJKwKrjmtMnhnWw7X65vpxa?dl=0

## Description
This project utilizes deep learning techniques, specifically a ResNet50 model, to perform binary classification on a dataset. The goal is to identify patterns within images and make predictions regarding the target classes.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Dependencies](#dependencies)
- [License](#license)

## Installation
To run this project, ensure you have Python and the required libraries installed. You can install the necessary dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Usage
1. **Data Preparation:**
   - Organize your dataset into the 'Train' and 'Test' directories.
   - Make sure the images are appropriately labeled.

2. **Model Configuration:**
   - Adjust parameters like `img_size`, `batch_size`, and the ResNet50 model configuration in the script.

3. **Training:**
   - Run the script `train_model.py` to train the model.

4. **Evaluation:**
   - The script evaluates the model on the test set and prints metrics like accuracy, confusion matrix, and classification report.

5. **Visualization:**
   - ROC curve and AUC are plotted to visualize model performance.

## Results
The trained model achieved a test accuracy of approximately 86.98%. Here are some key results:

- Confusion Matrix:
  ```
  [[566  49]
   [145   8]]
  ```

- Classification Report:
  ```
                precision    recall  f1-score   support

           0       0.80      0.92      0.85       615
           1       0.14      0.05      0.08       153

    accuracy                           0.75       768
   ```

- Sensitivity: 0.0523
- Specificity: 0.9203
- ROC curve with an AUC of approximately 0.67.

## Dependencies
- Python 3.x
- TensorFlow
- Matplotlib
- Numpy
- Scikit-learn

