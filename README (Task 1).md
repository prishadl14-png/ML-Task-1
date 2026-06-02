# SPML Task 1: Gradio Web App (SPML_Task_1.ipynb)

## Overview
This notebook deploys the custom PyTorch model trained on the Fashion-MNIST dataset into an interactive web interface using **Gradio**. 

## Requirements
Before running this deployment notebook, you must have:
1. Successfully executed the training notebook.
2. The generated `model_weights.pkl` file available in your working directory.

Required libraries:
* `torch`
* `torchvision`
* `gradio`

## Running the Web Interface
1. Open the notebook in your preferred environment (e.g., Google Colab or local Jupyter environment).
2. Ensure `model_weights.pkl` is in the same directory.
3. Run all cells. 
4. The Gradio cell will start a local server and generate a public `gradio.live` link (valid for 72 hours).
5. Click the public link to access the chatbot-style interface and interact with your trained fashion classifier.

## Deployment Notes
For permanent hosting, the Gradio application can be deployed to Hugging Face Spaces using the `gradio deploy` command from your terminal.
