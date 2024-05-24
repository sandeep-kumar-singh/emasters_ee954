# README for EE954 Assignment

## Code structure
TBD

---

## How to Run
TBD

---

## Report: PyTorch-based Neural Network Training and Testing

### Part 1: Data Preparation

The code consists of two sections for data preparation: one using PyTorch (`torch`) and the other using `numpy`.

- **PyTorch Data Preparation**:
  - It downloads the Fashion MNIST dataset and splits it into training, validation, and test datasets.
  - Data loaders are created for each dataset to facilitate batch-wise training.

- **Numpy Data Preparation**:
  - It downloads and extracts the Fashion MNIST dataset using `numpy`.
  - Splits the training set into training and validation subsets.
  - Prints the shapes of the training, validation, and test datasets.

### Part 2: Model Definition and Training

#### Multi-Layer Perceptron (MLP)
- A custom implementation of a multi-layer perceptron (MLP) is defined.
- It consists of dense layers with ReLU activation.
- The model is trained using the training and validation datasets.
- Training progress (loss and accuracy) is printed for each epoch.

#### Backbone CNN Model
- A convolutional neural network (CNN) model is defined as a backbone for feature extraction.
- It consists of 5 convolutional layers followed by ReLU activation and max-pooling layers.
- The backbone CNN is trained and validated using the Fashion MNIST dataset.

### Part 3: Integration of Backbone CNN with MLP

- Features are extracted from the trained backbone CNN model.
- These features are used to train the MLP for classification.
- The MLP is trained and validated using the extracted features.

### Results and Conclusion

- The backbone CNN and MLP are trained and tested separately.
- Training and validation loss, accuracy, and testing accuracy are reported.
- The trained models (backbone CNN and MLP) are saved for future use.

---

This code demonstrates a comprehensive pipeline for training and testing neural networks using PyTorch, encompassing data preparation, model definition, training, and testing. The combination of a backbone CNN for feature extraction and an MLP for classification provides flexibility and performance in handling the Fashion MNIST dataset.
