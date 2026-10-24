# Handwritten Digit Classification using CNN and RNN

This project demonstrates handwritten digit recognition on the MNIST dataset using two deep learning models:

- Convolutional Neural Network (CNN)
- Recurrent Neural Network (RNN) using LSTM

The notebook compares the performance of both models and visualizes the confusion matrices for evaluation.

## Project Overview

The MNIST dataset contains grayscale images of handwritten digits (0-9). The model learns to classify each image into one of 10 classes.

This implementation uses:

- PyTorch
- Torchvision
- Matplotlib
- Seaborn
- scikit-learn
- Pandas
- NumPy

## Repository Contents

- `handwritten_digit_classification_using_cnn_and_rnn.ipynb` — main notebook containing data loading, model definitions, training, evaluation, and visualizations

## Requirements

Install the required libraries before running the notebook:

```bash
pip install torch torchvision matplotlib seaborn scikit-learn pandas numpy
```

## How to Run

1. Open the notebook in Jupyter or VS Code.
2. Run all cells in sequence.
3. The notebook will:
   - download the MNIST dataset
   - train the CNN model
   - train the RNN model
   - print accuracy for both models
   - generate confusion matrix plots

## Model Architecture

### CNN

The CNN model includes:

- 2 convolutional layers
- ReLU activations
- Max pooling layers
- Fully connected layers for classification

### RNN

The RNN model uses an LSTM layer:

- input size: 28
- hidden size: 128
- 2 LSTM layers
- final fully connected layer for 10 digit classes

## Training Details

- Optimizer: Adam
- Loss function: CrossEntropyLoss
- Learning rate: 0.001
- Epochs: 5
- Batch size: 100

## Example Results

The notebook reports final accuracies around:

- CNN: approximately 99.02%
- RNN: approximately 98.72%

These results show that both models perform very well on MNIST, with the CNN slightly outperforming the RNN in this setup.

## License

This project is distributed under the MIT License unless otherwise stated.

## Acknowledgments

- MNIST dataset from the official handwritten digits benchmark
- PyTorch and Torchvision ecosystem for deep learning tooling

## Notes

The notebook trains both models in the same environment and compares their classification performance. It is a good reference for learning:

- deep learning with CNNs
- sequence modeling with LSTMs
- training loops in PyTorch
- model evaluation and confusion matrices
