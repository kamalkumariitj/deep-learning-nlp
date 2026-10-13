# Deep Learning - NLP Flower Classification Notebook

## Author
- Chaurasia Kamalkumar Lallanprasad
- Roll Number: G25AIT2028

## Notebook
- `g25ait2028-deep-learning-nlp-flower.ipynb`

## Overview
This notebook demonstrates a simple deep learning-style binary classification problem using a single neuron with a sigmoid activation function. The goal is to classify flowers based on two features:

- Petal length
- Petal width

The dataset contains labeled points where:
- `0` represents one flower class (blue)
- `1` represents the other flower class (red)

The notebook visualizes the data, trains a lightweight neural network, and predicts the class of a mystery flower.

## What the notebook does
1. Loads and plots flower feature data
2. Visualizes the points on a 2D graph
3. Defines a sigmoid activation function and its derivative
4. Trains a simple neural network using gradient descent
5. Tracks the training cost to confirm learning
6. Predicts the category of a mystery flower based on its dimensions

## Dataset
The notebook uses a small handcrafted dataset:

```python
data = [[3, 1.5, 1],
        [2, 1, 0],
        [4, 1.5, 1],
        [3, 1, 0],
        [3.5, .5, 1],
        [2, .5, 0],
        [5.5, 1, 1],
        [1, 1, 0]]
```

The mystery flower is defined as:

```python
mystery_flower = [4.5, 1]
```

## Model
A basic single-layer perceptron is used:

- Inputs: length, width
- Weights: `w1`, `w2`
- Bias: `b`
- Activation: sigmoid

The model learns the decision boundary by minimizing squared error using gradient descent.

## Dependencies
To run this notebook, install the following:

- Python 3
- Jupyter Notebook / JupyterLab
- NumPy
- Matplotlib

## How to run
1. Open the notebook in Jupyter.
2. Run all cells in order.
3. Observe the plots and printed prediction output.

## Expected output
The notebook plots:
- The original flower data points
- The sigmoid curve
- The training cost reduction over iterations
- The final decision boundary in the feature space

The final prediction for the mystery flower is printed as a probability value:
- A value close to `0` means blue class
- A value close to `1` means red class

## Conclusion
This notebook is a beginner-friendly introduction to a neural network trained for binary classification using simple handcrafted data. It helps illustrate how a basic machine learning model learns to separate classes in a 2D feature space.
