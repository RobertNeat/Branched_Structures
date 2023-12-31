# Neural Network with Tree-like Structure

## Overview

This repository contains code implementing a dense neural network with a tree-like architecture for feature extraction from images. Inspired by the Inception architecture, this model aims to use a functional interface from the Keras library to construct a tree structure.

## Implementation Details

### Modules and Structure

The primary function `add_module` constructs a tree structure by defining branches, each comprising various dense layers. This design allows for multiple paths for feature extraction at different levels of detail.

### Model Construction

1. **Branching:** The branches are added to the neural network using the defined modules.
2. **Common Layers:** Both before and after branching, common layers such as Reshape, BatchNormalization, and Average pooling are applied.

## Usage

### Dependencies

- This code requires Keras library to be installed (`pip install keras.utils`).

### Running the Code

- Ensure the necessary dependencies are installed.
- Execute the code in a Python environment that supports Keras, such as Jupyter Notebook.

### Visualization

- The code provides functionality to visualize the network structure using `plot_model`.

## Example Usage

```python
# Assuming necessary imports and input_tensor definition
# ... (code snippet from the provided notebook)

# Branching:
output_tensor = add_module(input_tensor)

# Common layers (after merging branches):
output_tensor = Average()(output_tensor)

model1 = Model(inputs=input_tensor, outputs=output_tensor)
model1.compile(loss='categorical_crossentropy', metrics='accuracy', optimizer='adam')

# Visualizing network structure
from tensorflow.keras.utils import plot_model
plot_model(model1, show_shapes=True)

```
### License

This code is provided under LICENSE.md, specifying the terms and conditions for its usage.
Contributors

    Robert Neat - Initial implementation (GitHub)

### Contact

For any inquiries or issues regarding this code, please contact the contributors.

## Launching Project

To run the project, you have a couple of options:

### Using Google Colab via Gist

Access the project through Google Colab using the Gist website. You can import the necessary data from the GitHub project resources. Use the following Gist link: [gist link here](https://gist.github.com/RobertNeat/dfed06fe43c30c459c785d988e11f307)

### Running Locally

If you prefer to run the project on your local machine, follow these steps:

1. **Clone the Repository**: Download the repository branch from GitHub.
2. **Local Environment**:
   - **DataSpell or PyCharm**: Open the project using DataSpell or PyCharm by JetBrains.
   - **Spyder IDE**: Alternatively, you can use Spyder IDE to work with the project.
3. **Dataset Requirements**:
   - Ensure that the dataset files are available and stored inside your project directory. This step is crucial to prevent any issues related to missing data.

Running the project locally allows you to explore the code and execute it in your preferred Python environment. If you encounter any problems, make sure to check the dataset's presence in your project directory.
