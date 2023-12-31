# ResNet Architecture Neural Network

## Description

This code implements a neural network using ResNet layers to construct a dense neural network via a functional interface. The ResNet architecture involves the utilization of skip connections (or residual connections) to mitigate the vanishing gradient problem in deeper networks.

## Files

- **lab8_resnet_architecture.ipynb**: Jupyter Notebook file generated in Colaboratory.
    - **[Original File](https://colab.research.google.com/gist/RobertNeat/6ac125b44f638c1b2475b073bb0daf14/lab8_resnet_architecture.ipynb)**

## Objective

The primary objective of this code:
- Construct a neural network using ResNet layers.
- Train and test the tensors inside the neural network model to evaluate accuracy and loss metrics.

## Libraries and Data

- **Libraries Used**:
    - Keras (for building the neural network)
    - NumPy (for array operations)
    - Pandas (for data manipulation)

- **Dataset Used**: MNIST
    - Loaded using Keras (`keras.datasets.mnist`)
    - Preprocessed for training and testing

## Architecture

- **ResNet Block Function**:
    - Defined to create ResNet blocks with convolutional layers, batch normalization, skip connections, and ReLU activation.

- **Model Construction**:
    - Constructs a neural network using a specified number of ResNet blocks.
    - Utilizes Dense layers with softmax activation.

- **Compilation**:
    - Compiles the model with categorical cross-entropy loss and Adam optimizer.

- **Training and Testing**:
    - Trains the model using the MNIST dataset for 10 epochs.

## Additional Features

- **Network Visualization**:
    - Utilizes `plot_model` from TensorFlow Keras to visualize the network structure with shapes.

- **Learning Curve**:
    - Generates learning curves (loss and accuracy) for the trained model over 10 epochs.

## Usage

- Ensure necessary libraries are installed (`Keras`, `NumPy`, `Pandas`, `TensorFlow`).
- Load the provided notebook in a compatible environment (e.g., Jupyter Notebook, Google Colab).
- Run each cell sequentially to execute the code blocks.
- Analyze the learning curves and network structure visualizations to understand the model's performance and architecture.

## Launching Project

To run the project, you have a couple of options:

### Using Google Colab via Gist

Access the project through Google Colab using the Gist website. You can import the necessary data from the GitHub project resources. Use the following Gist link: [gist link here](https://gist.github.com/RobertNeat/6ac125b44f638c1b2475b073bb0daf14)

### Running Locally

If you prefer to run the project on your local machine, follow these steps:

1. **Clone the Repository**: Download the repository branch from GitHub.
2. **Local Environment**:
   - **DataSpell or PyCharm**: Open the project using DataSpell or PyCharm by JetBrains.
   - **Spyder IDE**: Alternatively, you can use Spyder IDE to work with the project.
3. **Dataset Requirements**:
   - Ensure that the dataset files are available and stored inside your project directory. This step is crucial to prevent any issues related to missing data.

Running the project locally allows you to explore the code and execute it in your preferred Python environment. If you encounter any problems, make sure to check the dataset's presence in your project directory.
