# Image Captioning using hybrid CNN-LSTM Model

This project aims to generate descriptive captions for the given images by implementing a hybrid Convolutional Neural Network (CNN) - Long-Short Term Memory (LSTM) models. The project involves essential steps like Image pre-processing, Captions cleaning and Tokenization, Image Features Extraction, Model Building, Training and Evaluation, Fine-Tuning and Model Testing.

## Features

**Image Pre-processing**:
* Loaded the Flickr8k dataset and resized the images
* Reshaped the image data to pre process in RBG format
* Split the image name from the extension to only load the image name

**Features Extraction**
* Extracted the features using the VGG16 model
* Stored the extracted features using Pickle module for quicker use and future use

**Captions Cleaning and Tokenization**
* Loaded the captions text file, which contains 5 captions per each image
* Mapped each word to a unique integer using a tokenizer
* Pre-processed the captions like deleting digits, special characters, additional spaces and adding start and end tokens to the beginning and end of each caption

**Train/Test Split**
* Split the dataset into 90% for training and 10% for testing purposes
* Defined a batch generator which includes a padding sequence to normalizes the size of all captions to the max size for better results.

**Model Building** Evaluation
* Built the model using Tensorflow encoder-decoder architecture
* Summarized and plotted the model for numerical and visual representation of the model architecture

**Model Training**
* Trained the model over 20 epochs
* Added backpropagation layer to decrease loss
* Saved the trained model

**Model Evaluation**
* Evaluated the model using Bilingual Evaluation Understudy (BLEU) scores.

**Model Testing**
* Tested the model on an image and visualized the results
* First prints the actual captions of the image then prints a predicted caption of the image
