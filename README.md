
# Handwritten Digit Recognition using MNIST Dataset
## Project Description
This project implements a Multilayer Perceptron (MLP) using PyTorch to classify handwritten digits from the MNIST dataset.
The model is trained to recognize handwritten digits from 0 to 9 using a simple neural network architecture.
The project includes:
- Data preprocessing
- Model training
- Validation and testing
- Performance evaluation
- Visualization of accuracy and loss curves
- Experiment comparison using different activation functions and hyperparameters
---
# Dataset Information
The project uses the MNIST dataset provided by:
```python
torchvision.datasets.MNIST

Dataset Details:

* 60,000 training images
* 10,000 testing images
* Grayscale handwritten digit images
* Image size: 28 × 28 pixels

⸻

Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-learn

⸻

Data Preprocessing

The following preprocessing steps were applied:

* Convert images to tensors
* Normalize pixel values
* Split dataset into:
    * Training set
    * Validation set
    * Testing set

Normalization was applied using:

transforms.Normalize((0.1307,), (0.3081,))

⸻

Model Architecture

The implemented model is a simple Multilayer Perceptron (MLP).

Architecture:

Layer	Size
Input Layer	784
Hidden Layer	128 / 256
Output Layer	10

Activation Functions Used:

* ReLU
* Tanh

Loss Function:

* CrossEntropyLoss

Optimizer:

* Adam Optimizer

⸻

Experiments

Experiment 1

* Activation Function: ReLU
* Hidden Neurons: 128
* Learning Rate: 0.001

Results

* Test Accuracy: 97.18%

⸻

Experiment 2

* Activation Function: Tanh
* Hidden Neurons: 256
* Learning Rate: 0.01

Results

* Test Accuracy: 91.43%

⸻

Experiment Comparison

Experiment	Activation Function	Hidden Neurons	Learning Rate	Test Accuracy
Experiment 1	ReLU	128	0.001	97.18%
Experiment 2	Tanh	256	0.01	91.43%

⸻

Result Analysis

Experiment 1 achieved better performance because:

* ReLU activation function trained faster
* Lower learning rate improved training stability
* Validation loss decreased consistently

Experiment 2 showed lower performance because:

* High learning rate caused unstable learning
* Tanh activation trained slower than ReLU

⸻

Evaluation Metrics

The project includes:

* Test Accuracy
* Final Loss Value
* Confusion Matrix
* Classification Report

⸻

Visualizations

The project generates:

* Training Loss Curve
* Validation Loss Curve
* Accuracy Curve
* Experiment Comparison Graphs

⸻

Sample Output

The model predicts handwritten digits correctly with high accuracy.

Final Best Accuracy:

97.18%

⸻

How to Run the Project

1. Install Requirements

pip install -r requirements.txt

2. Run the Notebook

Open the notebook in Google Colab or Jupyter Notebook and run all cells.

⸻

Project Structure

project/
│
├── Neural Network Project.ipynb
├── README.md
└── report.tex

⸻

Author

Mostafa Badawe Fouad
ID: 2023019029
AI3

⸻

