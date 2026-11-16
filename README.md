# Fashion-MNIST Image Classification Using CNN

## Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify clothing images from the Fashion-MNIST dataset into 10 categories.

The objective is to explore image preprocessing, convolutional feature extraction, deep learning model training, and multiclass classification performance.

## Dataset

The project uses the [Fashion-MNIST dataset](https://github.com/zalandoresearch/fashion-mnist).

- Total images: 70,000
- Training images: 60,000
- Testing images: 10,000
- Image dimensions: 28 × 28 pixels
- Image format: Grayscale
- Number of classes: 10

### Classification Categories

1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn

## CNN Architecture

The model consists of:

1. Input layer (28 × 28 × 1)
2. Conv2D (32 filters, 3 × 3, ReLU)
3. MaxPooling2D (2 × 2)
4. Conv2D (64 filters, 3 × 3, ReLU)
5. MaxPooling2D (2 × 2)
6. Flatten
7. Dense (128 neurons, ReLU)
8. Dropout (0.3)
9. Dense (10 neurons, Softmax)

### Training Configuration

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Epochs: 5
- Batch Size: 128
- Validation Split: 10%

## Implementation Workflow

1. Dataset loading and exploration
2. Visualisation of sample images
3. Image normalisation and preprocessing
4. CNN architecture development
5. Model training and validation
6. Test-set evaluation
7. Accuracy and loss visualisation
8. Confusion matrix and classification report
9. Individual image prediction

## Results

The model achieved the following performance:

| Metric | Result |
|---|---:|
| Training Accuracy | 89.58% |
| Validation Accuracy | 89.00% |
| Test Accuracy | 88.53% |
| Test Loss | 0.3145 |

The classification report shows varying performance across categories. The model performs particularly well on trousers, sandals, bags and sneakers, while shirts remain a more challenging category.

## How to Run

1. Clone this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Install TensorFlow and the other required libraries if necessary.
4. Execute the notebook cells sequentially.

The Fashion-MNIST dataset is loaded directly through TensorFlow/Keras.

## Future Improvements

- Experiment with additional convolutional layers.
- Increase training epochs.
- Explore hyperparameter tuning.
- Apply data augmentation.
- Investigate techniques to improve classification of visually similar categories.

## Project Context

Academic Machine Learning and Deep Learning implementation developed alongside undergraduate coursework.
