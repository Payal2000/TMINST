# Typeface MNIST (TMNIST) Character Recognition

This repository contains the implementation of a Convolutional Neural Network (CNN) for character recognition on the Typeface MNIST (TMNIST) dataset, an extension of the original MNIST dataset featuring digits in various Google font styles.

## Dataset Overview

The TMNIST dataset enriches the classic MNIST digit recognition task with the complexity of typeface variations, including 2,990 unique Google fonts. Each digit from 0-9 is represented across these diverse styles.

## Preprocessing Steps

- **Normalization**: Pixel values are normalized to a [0, 1] range to facilitate model convergence.
- **Reshaping**: The dataset is reshaped from flat vectors into 2D images to fit the input shape expected by CNNs.

## Model Architecture

The CNN model includes:

- Multiple convolutional layers to extract features from the typeface variations.
- Pooling layers to reduce spatial dimensions while preserving the most important features.
- Dense layers for classification, with dropout regularization to combat overfitting.

## Training Procedure

- **Loss Function**: Cross-entropy loss, ideal for multi-class classification problems.
- **Optimizer**: Adam, known for its adaptive learning rates and efficient training.
- **Batch Processing**: Mini-batch gradient descent for more efficient weight updates.

## Evaluation Metrics

- **Accuracy**: Overall correctness of the model.
- **Precision & Recall**: Measures of the model's exactness and completeness.
- **F1-Score**: The harmonic mean of precision and recall.
- **Confusion Matrix**: Visual tool to identify misclassifications.

## Post-Processing

Post-training analysis includes:

- Fine-tuning the model based on the evaluation metrics.
- Investigating misclassifications via confusion matrix analysis.
- Exploring advanced techniques like transfer learning for performance improvement.

## Deployment

The final model can be deployed for various applications, such as document digit recognition and typeface style transfer tasks.

## Getting Started

To get started with this project, clone the repository and install the required dependencies as listed in `requirements.txt`.

```bash
git clone https://github.com/your-username/tmnist-character-recognition.git
cd tmnist-character-recognition
pip install -r requirements.txt


