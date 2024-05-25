# README for EE954 Assignment

## Repository Organization
This project has following code (.ipynb) files:
1. `EE954_Assignment.ipynb` - This is the main code that implements both MLP and CNN models for classification of Fashion-MNIST datasets.
2. `archive/*TRYOUTS.ipynb` - These files contains code snippets for various experiments/trials that we done to arrive at the final solution in (1).

---

## Code Structure

### Import Dependencies
Imports all the dependencies required for the entire codebase.

### Part 1 - Data Preparation
The code consists of two sections for data preparation: one using PyTorch (`torch`) and the other using `numpy`.

- **Data Preparation (using pyTorch)**:
  - It downloads the Fashion MNIST dataset and splits it into training, validation, and test datasets.
  - Data loaders are created for each dataset to facilitate batch-wise training.

- **Data Preparation (using numpy)**:
  - It downloads and extracts the Fashion MNIST dataset using `numpy`.
  - Splits the training set into training and validation subsets.
  - Prints the shapes of the training, validation, and test datasets.

### Select Device for Executing the CNN/MLP Models
This helps select the device (CPU/GPU/MPS) for running models.

### MLP Model for Classification
- A custom implementation of a multi-layer perceptron (MLP) is defined.
- It consists of dense layers with ReLU activation.

### MLP - Model Training and Testing
- The model is trained using the training and validation datasets.
- Training progress (loss and accuracy) is printed for each epoch.
- MLP is executed for test dataset.

### CNN Model for Feature Extraction
- A convolutional neural network (CNN) model is defined as a backbone for feature extraction.
- It consists of 5 convolutional layers followed by ReLU activation and max-pooling layers.
- The backbone CNN is trained and validated using the Fashion MNIST dataset.

### Standalone CNN - Model Training and Testing
- Features are extracted from the trained backbone CNN model.
- These features are fed to an in-built Dense Network .
- The MLP is trained and validated using the extracted features.

### CNN and MLP Combined - Model Training and Testing
- Features are extracted from the trained backbone CNN model.
- These features are used to train the MLP for classification.
- The MLP is trained and validated using the extracted features.

---

## How to Run
`EE954_Assignment.ipynb` to be run in Google Colab.

### Standalone MLP
Run the code cells in following order:
1. Import Dependencies
2. Part 1 - Data Preparation > Data Preparation (using numpy)
3. MLP Model for Classification
4. MLP - Model Training and Testing

### Standalone CNN
Run the code cells in following order:
1. Import Dependencies
2. Part 1 - Data Preparation > Data Preparation (using numpy)
3. Select Device for Executing the CNN/MLP Models
4. CNN Model for Feature Extraction
5. Standalone CNN - Model Training and Testing

### Combined CNN and MLP
Run the code cells in following order:
1. Import Dependencies
2. Part 1 - Data Preparation > Data Preparation (using pyTorch)
3. Select Device for Executing the CNN/MLP Models
4. CNN Model for Feature Extraction
5. CNN and MLP Combined - Model Training and Testing
