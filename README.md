
# Face Mask Detection 😷
This project demonstrates a simple **Convolutional Neural Network (CNN) model** for detecting whether a person is wearing a face mask in an image. The model is trained and evaluated using a dataset from Kaggle. The entire workflow, from data acquisition and preprocessing to model training and making predictions on new images, is contained within a single Jupyter notebook.

## Table of Contents
- Features
- Model Architecture
- Prerequisites
- How to Use

## Features
- __Automatic Data Download:__ The notebook uses the Kaggle API to automatically download the necessary dataset.
- **Image Preprocessing:** Images are resized and normalized for consistent model input.
- **CNN Model:** A basic but effective CNN is built and trained from scratch using ```tensorflow.keras```.
- **Model Evaluation:** The model's performance is evaluated on a test set, and its training history (accuracy and loss) is visualized.
- **Predictive System:** The notebook includes code to make predictions on new, unseen images.

## Model Architecture
The CNN is designed to be straightforward and effective for this binary classification task. It consists of the following layers:

- A series of ```Conv2D``` and ```MaxPooling2D``` layers to extract features from the images.
- A ```Flatten``` layer to convert the 2D feature maps into a 1D vector.
- Two fully connected ```Dense``` layers with ```ReLU``` activation.
- ```Dropout``` layers to prevent overfitting.
- An output ```Dense``` layer with ```Sigmoid``` activation to produce the final classification.
- The model is compiled with the ```adam``` optimizer and ```sparse_categorical_crossentropy``` as the loss function.

## Prerequisites
To run this project, you need a Kaggle account to download the dataset. You also need a Python environment with the following libraries installed:

- ```tensorflow```
- ```keras```
- ```kaggle```
- ```numpy```
- ```matplotlib```
- ```opencv-python```
- ```Pillow```
- ```scikit-learn```

The notebook includes a cell to install ```kaggle``` if it is not already present in your environment.

## How to Use
1. Clone the repository to your local machine:

git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)

2. Download your Kaggle API key. Go to your Kaggle account settings and click "Create New API Token." This will download a file named ```kaggle.json```.

3. Place the ```kaggle.json``` file in the same directory as the Jupyter notebook.

4. Run the ```Face_mask_detection.ipynb``` notebook in your preferred environment (e.g., Jupyter, VS Code, Google Colab). The notebook is designed to be executed cell-by-cell.

5. Make Predictions:

- The final section of the notebook is a predictive system.

- Provide the path to any image you want to test, and the model will predict if the person is wearing a mask.


