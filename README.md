![Cover image](https://github.com/nileshparab42/Alzheimers-Disease-Classification/blob/main/Assets/Alzimer.png)

# Alzheimer's Classification(Using Vgg16)

The Alzheimer's Classifier is a deep learning model developed using the Vgg16 architecture. This classifier is specifically designed to assess and categorize brain imaging data to identify patterns associated with Alzheimer's disease. By utilizing VGG16's deep layers for feature extraction, the classifier can effectively differentiate between brain scans from individuals with Alzheimer's disease and those without. This enables early and accurate detection of Alzheimer's-related changes, potentially assisting medical professionals in diagnosing and managing the disease more effectively.

## Background About Dataset

### Context
The Data is hand collected from various websites with each and every labels verified.

### Content
The data consists of MRI images. The data has four classes of images both in training as well as a testing set:

1. Mild Demented
2. Moderate Demented
3. Non Demented
4. Very Mild Demented

## ResNet50 architecture 

![Cover image](https://neurohive.io/wp-content/uploads/2018/11/vgg16-1-e1542731207177.png)

The VGG16 architecture is a deep convolutional neural network (CNN) model designed for image classification tasks. It was developed by the Visual Geometry Group (VGG) at the University of Oxford. VGG16 is known for its simplicity and effectiveness, making it a widely used architecture in computer vision.

Key characteristics of the VGG16 architecture include:

Layer Depth: VGG16 consists of 16 layers, which include 13 convolutional layers and 3 fully connected layers. The convolutional layers are stacked in a sequential manner, with smaller 3x3 filters, which helps capture intricate features in the input images.

**Filter Size and Stride:** The convolutional layers use small 3x3 filters with a stride of 1, ensuring that the spatial dimensions of the input are preserved while extracting features.

**Pooling Layers:** After a few convolutional layers, VGG16 uses max-pooling layers with 2x2 filters and a stride of 2 to reduce the spatial dimensions and downsample the feature maps.

**Fully Connected Layers:** The final layers of VGG16 consist of three fully connected layers, which are followed by a softmax activation function for class prediction in the case of image classification.

**Activation Function:** Rectified Linear Unit (ReLU) activation functions are used throughout the network to introduce non-linearity.

**Parameters:** Due to its depth and large number of filters, VGG16 has a high number of trainable parameters. This makes it more prone to overfitting when working with limited training data.

**Pre-Trained Models:** VGG16 is often used as a pre-trained model on large image datasets like ImageNet. Researchers commonly fine-tune this pre-trained model on specific tasks to leverage the learned features.

VGG16's simplicity and modular structure make it a great starting point for many computer vision projects, although its depth can also lead to increased computational requirements compared to more lightweight architectures.

![Cover image](https://github.com/nileshparab42/Alzheimers-Disease-Classification/blob/main/Assets/graph.png)

### Model Summary

Total params: 14,714,688
Trainable params: 14,714,688
Non-trainable params: 0


### Optimizers Parameters

loss='categorical_crossentropy'
optimizer='adam'
metrics=['accuracy']

## Contributing

We appreciate contributions from the community to enhance model. If you'd like to contribute, please follow these steps:

1. Fork the repository on GitHub.

2. Create a new branch from the "main" branch.

3. Make your desired changes and improvements in the code.

4. Test your changes thoroughly.

5. Create a pull request and provide a detailed description of the changes you made.

6. Our team will review your pull request, and if everything looks good, we'll merge it into the main repository.


## Installation

### Get the Alzheimers Classifier Repository now.

To download a Alzheimers Classifier project, you can use the git clone command. This command creates a copy of the repository in a new directory on your local machine.
```
git clone https://github.com/nileshparab42/Alzheimers-Disease-Classification/tree/main
```
To set up the project, you can use the pip command to install the required packages specified in the requirements.txt file.
```
pip install -r requirements.txt
```
This will install all of the required packages for the project. If you are using a virtual environment for the project, you should activate the environment before running this command.
```
pip install virtualenv
virtualenv myenv
source myenv/bin/activate
pip install -r requirements.txt
```
This will create a new virtual environment called myenv, activate it, and then install the required packages.

You can also specify the notebook file location or the working directory, after the command "jupyter notebook" or "jupyter lab" like:
```
jupyter notebook /path/to/notebook/directory
```
or
```
jupyter lab /path/to/notebook/directory
```
It will open the Jupyter notebook or lab in the specified directory, making it easier to navigate to the notebook you want to open.


## Authors

- [Nilesh Parab](https://github.com/nileshparab42) (Project Lead) - [Website](https://nileshparab10.blogspot.com/)
  

## Acknowledgements

- This project was inspired by the work of the [CodeWthHarry](https://www.youtube.com/@CodeWithHarry).
- We also used resources and tools from the [GeeksforGeeks](https://www.geeksforgeeks.org/speech-recognition-in-python-using-google-speech-api/) to develop and test our project.