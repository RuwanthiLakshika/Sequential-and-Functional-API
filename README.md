# TensorFlow Keras Models Overview

This README provides an overview of various Keras models using both Sequential and Functional APIs as demonstrated in the Jupyter Notebook.

## Sequential API

The Sequential API allows for the creation of models layer-by-layer in a step-by-step fashion.

- **Model Structure**:
  - Dense layer with 64 units, ReLU activation, and input shape of (2,)
  - Dense layer with 16 units, ReLU activation
  - Dense layer with 1 unit, Sigmoid activation

## Functional API

The Functional API offers more flexibility and is used for models that require non-linear topology, shared layers, or multiple inputs/outputs.

### Single Input & Single Output

- **Model Structure**:
  - Input layer with shape (2,)
  - Two Dense layers with ReLU activation (64 and 16 units)
  - Output Dense layer with 1 unit, Sigmoid activation

### Multiple Inputs & Single Output

- **Model Structure**:
  - Two Input layers with shapes (2,) and (5,)
  - Dense and Normalization layers
  - Concatenation of intermediate layers
  - Output Dense layer with 1 unit, Sigmoid activation

### Single Input & Multiple Outputs

- **Model Structure**:
  - Input layer with shape (2,)
  - Two Dense layers with ReLU activation (16 and 32 units)
  - Two Output Dense layers with Sigmoid and Softmax activations

### Multiple Inputs & Multiple Outputs

- **Model Structure**:
  - Two Input layers with shapes (2,) and (5,)
  - Dense and Normalization layers
  - Concatenation of intermediate layers
  - Two Output Dense layers with Sigmoid and Softmax activations

## Activation Function

The `Dense` layer includes an activation function that applies an element-wise operation. The default activation is linear, but other functions like ReLU and Sigmoid are used in this notebook.

## Usage

To use these models, ensure you have TensorFlow installed and import the necessary modules as shown in the notebook.

