# MiniDigitAI

A simple handwritten digit recognition project built using a Convolutional Neural Network (CNN) and PyTorch.

## Project Overview

MiniDigitAI learns to recognize handwritten digits from 0 to 9 using the MNIST dataset.

The project covers the complete basic machine learning workflow:

* Dataset loading
* Image preprocessing
* Data visualization
* CNN model building
* Model training
* Model evaluation
* Error analysis
* Model saving and loading
* Inference on unseen images

## Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-learn
* Kaggle GPU

## Dataset

The project uses the **MNIST handwritten digit dataset**.

* Training samples: 60,000
* Testing samples: 10,000
* Image size: 28 × 28 pixels
* Classes: 10 digits (0–9)

## Model Architecture

The CNN contains:

1. Convolutional Layer — 1 → 16 channels
2. ReLU activation
3. Max Pooling
4. Convolutional Layer — 16 → 32 channels
5. ReLU activation
6. Max Pooling
7. Fully Connected Layer — 1568 → 128
8. Fully Connected Layer — 128 → 10

## Training

The model was trained using:

* Loss Function: Cross Entropy Loss
* Optimizer: Adam
* Learning Rate: 0.001
* Batch Size: 64

The project experimented with different training durations and compared the resulting model performance.

## Results

The final model was evaluated on the MNIST test dataset.

**Final Test Accuracy:** `99.04%`

**Test Samples:** `10,000`

The exact result is recorded in the Kaggle notebook.

## Error Analysis

Incorrect predictions were collected and visualized to understand which handwritten digits were difficult for the model.

A confusion matrix was also generated to analyze classification performance across all ten digit classes.

## Model

The trained model is saved as:

```text
mini_digit_cnn_final.pth
```

The model can be loaded using PyTorch and used for inference on MNIST-format images.

## Project Structure

```text
MiniDigitAI/
│
├── MiniDigitAI.ipynb
├── mini_digit_cnn_final.pth
└── README.md
```

## Future Improvements

Possible improvements include:

* Add a web-based digit drawing interface
* Add real-time prediction
* Experiment with data augmentation
* Compare different CNN architectures
* Deploy the model as an API

## Learning Outcome

This project helped me understand the complete CNN workflow, from loading and preprocessing image data to training, evaluating, saving, loading, and using a trained deep learning model for prediction.
