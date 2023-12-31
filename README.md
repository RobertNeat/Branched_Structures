# Neural Network with Lambda Layers

## Objective

The main objective of this code is to demonstrate the construction of a neural network using lambda layers to build a dense neural network using the functional interface in Keras.

## Files

- `lab8_lambda_layer.ipynb`: Jupyter Notebook containing the code.
- `README.md`: This file, providing an overview of the code and its objectives.

## Usage

### Libraries Used
- `keras`: for building and training neural networks.
- `numpy`: for array operations.
- `pandas`: for data manipulation.
- `tensorflow`: as the backend for Keras.

### Setup
- Ensure the necessary libraries are installed (e.g., Keras, TensorFlow, NumPy, Pandas).
- Access the [original file](https://colab.research.google.com/gist/RobertNeat/656de14f1b0eae791261cd040613a3d0/lab8_lambda_layer.ipynb) via Colab for detailed execution and data access.

### Description
1. **Loading Data**: MNIST dataset is loaded and preprocessed for training and testing.
2. **Neural Network Construction**:
   - Input layer created based on the shape of training data.
   - Addition of a 2D convolutional layer with 32 filters of size 3x3.
   - Integration of a Lambda layer using the Mish activation function.
   - Flattening of the output tensor.
   - Addition of a Dense layer with 10 units and softmax activation.
   - Model compilation with categorical cross-entropy loss, accuracy metrics, and Adam optimizer.
3. **Training and Testing**:
   - Model training on the provided training data for 8 epochs.
   - Testing on the provided test batch.
4. **Network Learning Curve**:
   - Generation of plots showcasing loss and accuracy metrics during training.

## Launching Project

To run the project, you have a couple of options:

### Using Google Colab via Gist

Access the project through Google Colab using the Gist website. You can import the necessary data from the GitHub project resources. Use the following Gist link: [gist link here](https://gist.github.com/RobertNeat/656de14f1b0eae791261cd040613a3d0)

### Running Locally

If you prefer to run the project on your local machine, follow these steps:

1. **Clone the Repository**: Download the repository branch from GitHub.
2. **Local Environment**:
   - **DataSpell or PyCharm**: Open the project using DataSpell or PyCharm by JetBrains.
   - **Spyder IDE**: Alternatively, you can use Spyder IDE to work with the project.
3. **Dataset Requirements**:
   - Ensure that the dataset files are available and stored inside your project directory. This step is crucial to prevent any issues related to missing data.

Running the project locally allows you to explore the code and execute it in your preferred Python environment. If you encounter any problems, make sure to check the dataset's presence in your project directory.
