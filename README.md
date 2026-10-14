# PneumoDetect — Chest X-Ray Classification

A machine learning project that classifies chest X-ray images into **NORMAL** and **PNEUMONIA** categories using logistic regression implemented with Python and NumPy.

## Overview

This project explores binary image classification using concepts from Pattern Recognition and Machine Learning (PRML). It uses image preprocessing and a logistic regression model trained through gradient descent to predict the class of a chest X-ray image.

## Features

- **Image preprocessing:** Converts images to grayscale, resizes them to 64 × 64 pixels, and normalizes pixel values.
- **Feature extraction:** Flattens each image into a 4,096-dimensional feature vector.
- **Logistic regression:** Uses a sigmoid function to estimate class probabilities.
- **Model training:** Implements binary cross-entropy loss, analytical gradient computation, and gradient descent.
- **Performance evaluation:** Calculates accuracy, precision, recall, and F1-score.
- **Visualization:** Plots training and validation loss curves and visualizes the learned model weights as a heatmap.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Pillow (PIL)
- Google Colab

## Methodology

1. **Data preprocessing:** Load chest X-ray images, convert them to grayscale, resize them, and normalize pixel intensities.
2. **Feature representation:** Flatten each 64 × 64 image into a vector containing 4,096 features.
3. **Model initialization:** Initialize the logistic regression weights and bias.
4. **Training:** Compute predictions using the sigmoid function and update model parameters using gradient descent to minimize binary cross-entropy loss.
5. **Evaluation:** Calculate classification metrics on the validation dataset.
6. **Visualization:** Examine loss convergence and visualize the spatial distribution of learned weights.

## Evaluation Metrics

The model evaluates its predictions using:

- Accuracy
- Precision
- Recall
- F1-score

Training and validation loss curves are also plotted to observe optimization behavior.

## Running the Project

The original implementation was developed in Google Colab.

1. Open the Python script or notebook in Google Colab.
2. Provide the dataset in the expected directory structure.
3. Update the training and validation dataset paths in the code.
4. Install the required dependencies if they are not already available.
5. Run the code to preprocess the images, train the model, calculate evaluation metrics, and generate visualizations.

### Expected Dataset Structure

```text
dataset/
├── train/
│   ├── NORMAL/
│   └── PNEUMONIA/
└── val/
    ├── NORMAL/
    └── PNEUMONIA/
```

The dataset is not included in this repository. Ensure that you have permission to use and redistribute any dataset you choose.

## Limitations

- Each image is represented by flattened pixel intensities rather than learned spatial features.
- Logistic regression is a relatively simple model for image classification.
- Performance depends on the dataset, preprocessing, and training configuration.
- This project is for educational purposes and is not intended for clinical diagnosis or medical decision-making.

## Acknowledgements

Developed as part of academic work related to Pattern Recognition and Machine Learning (PRML).

## Disclaimer

PneumoDetect is an educational machine learning project. Its predictions must not be used as a substitute for professional medical assessment.
