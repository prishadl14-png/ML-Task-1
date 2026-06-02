# SPML Task 1: Fashion-MNIST Classification & Gradio App

This repository contains the solution for SPML Task 1. The project involves training a custom neural network on the Fashion-MNIST dataset using PyTorch and deploying it via an interactive Gradio web interface.

## Project Overview

The project is split into two main Jupyter Notebooks:

### 1. Model Training (`SPML_Task1_Base_(1).ipynb`)
This notebook handles the data pipeline, model architecture, training, and evaluation.
* **Dataset:** Fashion-MNIST.
* **Architecture:** A custom PyTorch neural network featuring two parallel branches with a skip connection, which are then concatenated before the final output layer.
* **Outputs Generated:** * `model_weights.pkl`: The saved model weights after training.
    * `submission.csv`: Generated predictions on the test set.
    * `training_curves.png`: Visualization of the loss and accuracy over epochs.
    * `confusion_matrix.png`: Visual evaluation of the model's classification performance.

### 2. Gradio Deployment (`SPML_Task_1.ipynb`)
This notebook loads the trained model weights and provides a web-based user interface using **Gradio**.
* Allows users to interact with the model seamlessly.
* Generates a public share link for easy access and can be deployed permanently to Hugging Face Spaces.

## Requirements

To run these notebooks, you will need the following Python libraries:
* `torch`
* `torchvision`
* `gradio`
* `matplotlib`
* `pandas`
* `numpy`
* `scikit-learn`

## Instructions to Run

1. **Train the Model:**
   * Open `SPML_Task1_Base_(1).ipynb` (preferably in Google Colab with a GPU accelerator like T4).
   * Run all cells to execute the training loop.
   * Ensure that the artifact files (especially `model_weights.pkl`) are saved successfully in your working directory.

2. **Launch the Web Interface:**
   * Open `SPML_Task_1.ipynb`.
   * Ensure the previously generated `model_weights.pkl` is in the same directory or accessible path.
   * Run all cells. The Gradio cell will output a local and public URL (e.g., `https://xxxx.gradio.live`). Click the link to use the interactive app.

