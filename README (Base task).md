# SPML Task 1: Model Training (SPML_Task1_Base_(1).ipynb)

## Overview
This notebook is dedicated to training a custom neural network on the Fashion-MNIST dataset using PyTorch. 

## Model Architecture
The architecture is specifically designed for image classification tasks with the following characteristics:
* **Dual-Branch System:** The network splits the input into two parallel branches to extract different sets of features.
* **Skip Connections:** Incorporates skip connections to preserve spatial information through the network layers.
* **Concatenation:** Features from both branches are concatenated before being passed to the final fully connected classification layer.

## Requirements & Setup
To run this notebook, you will need the following dependencies:
* `torch`
* `torchvision`
* `matplotlib`
* `pandas`
* `numpy`
* `scikit-learn`

It is highly recommended to run this notebook in Google Colab with a T4 GPU (or equivalent) for accelerated training.

## Outputs and Artifacts
Executing the notebook will produce the following files:
1. `model_weights.pkl`: The saved PyTorch model weights (state dictionary), which are essential for running the Gradio application later.
2. `submission.csv`: The model's target predictions on the test dataset.
3. `training_curves.png`: A graphical plot showing training loss and accuracy over the iterations/epochs.
4. `confusion_matrix.png`: A visual evaluation metric showing the model's accuracy across all 10 fashion classes.
