# DenseNet Architecture for Neural Networks

This code implements a DenseNet structure for building a neural network using the Keras library's functional interface. The DenseNet architecture used is described below:

![DenseNet Architecture](insert_image_link_here)

## Objective
The main objective of this code is to create a neural network utilizing DenseNet layers. The process involves:
1. Loading and preparing the MNIST dataset for training and testing.
2. Defining DenseNet blocks to construct the network.
3. Training the constructed neural network and evaluating its accuracy and loss metrics.

## Files
- `lab8_densenet_architecture.ipynb`: This Jupyter Notebook contains the code for implementing the DenseNet architecture.

## Usage
1. **Data Loading and Preprocessing:**
    - The MNIST dataset is loaded and separated into training and testing sets.
    - Data preprocessing includes expanding dimensions and one-hot encoding categorical labels.

2. **Building the DenseNet Blocks:**
    - The `block_DenseNet` function defines the structure of each DenseNet block used in the network.

3. **Constructing the Neural Network:**
    - The code constructs a neural network using the defined DenseNet blocks and additional layers.
    - Model compilation involves specifying loss, metrics, and optimizer.

4. **Training and Evaluation:**
    - The model is trained using the training data and evaluated using the test dataset.
    - Learning curves depicting loss and accuracy across epochs are generated.

## Requirements
- Keras
- NumPy
- Pandas
- Matplotlib

## Launching Project

To run the project, you have a couple of options:

### Using Google Colab via Gist

Access the project through Google Colab using the Gist website. You can import the necessary data from the GitHub project resources. Use the following Gist link: [gist link here](https://gist.github.com/RobertNeat/1721c6f1ee66715ea46a0216e463d900)

### Running Locally

If you prefer to run the project on your local machine, follow these steps:

1. **Clone the Repository**: Download the repository branch from GitHub.
2. **Local Environment**:
   - **DataSpell or PyCharm**: Open the project using DataSpell or PyCharm by JetBrains.
   - **Spyder IDE**: Alternatively, you can use Spyder IDE to work with the project.
3. **Dataset Requirements**:
   - Ensure that the dataset files are available and stored inside your project directory. This step is crucial to prevent any issues related to missing data.

Running the project locally allows you to explore the code and execute it in your preferred Python environment. If you encounter any problems, make sure to check the dataset's presence in your project directory.
