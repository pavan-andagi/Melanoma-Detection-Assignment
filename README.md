### Introduction
In this project, you will design a multiclass classification model using a custom convolutional neural network (CNN) implemented with TensorFlow.

### Problem Description
The goal is to develop a CNN-based model capable of accurately identifying melanoma, a type of cancer that can be fatal if not diagnosed early. Melanoma contributes to 75% of deaths caused by skin cancer. An automated solution that evaluates images to identify melanoma can significantly reduce the manual effort required in diagnosis, aiding dermatologists in their work. The dataset comprises 2,357 images of both malignant and benign oncological conditions, curated from the International Skin Imaging Collaboration (ISIC). These images were classified based on ISIC's standards, with the subsets containing equal numbers of images, except for melanomas and moles, which are slightly overrepresented.

### General Objective
The objective is to develop a model that accurately predicts demand for shared bikes based on available independent variables. This model will enable management to understand how demand fluctuates with different features, guiding their strategies to align supply with customer expectations. Additionally, this model will offer insights into demand dynamics in new markets.

### Dataset Details
The data used for training and testing the model is provided in the CNN_assignment.zip file.

Source: The dataset contains 2,357 images of malignant and benign conditions, sourced from the International Skin Imaging Collaboration (ISIC).
Preprocessing: To address class imbalance, the Python package Augmentor (see Augmentor Documentation) was utilized to augment the dataset, ensuring all classes have sufficient samples.

### Model Architecture
Rescaling Layer: Normalizes input data by scaling pixel values from [0, 255] to [0, 1].
Convolutional Layer: Applies a convolution operation, reducing input dimensions while extracting features from the input data. This operation compresses regions of the image into smaller, meaningful representations.
Pooling Layer: Reduces the size of feature maps, decreasing the computational complexity of the network. It summarizes features within specific regions of the feature map generated by the convolutional layer.
Dropout Layer: Introduces random deactivation of a fraction of neurons during training to prevent overfitting.
Flatten Layer: Converts the multidimensional output of convolutional layers into a one-dimensional array for input into dense layers.
Dense Layer: A fully connected layer where each neuron connects to all neurons in the previous layer.
Activation Functions:
ReLU: Outputs the input value if positive, otherwise returns zero, helping with faster learning and mitigating the vanishing gradient problem.
Softmax: Ensures output values are probabilities that sum to one, used for classification tasks with multiple classes.

### Conclusion
The CNN model was trained over approximately 20 epochs and evaluated over 50 epochs, achieving an accuracy of 92%. Detailed steps and results can be found in the Python notebook Melanoma_Detection_Assignment.ipynb under the "Train the Model" section.

### Contact
Created by: Pavan Andagi
