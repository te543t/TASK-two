# Image Classification Using Google Teachable Machine Model in Google Colab

## Overview

This project demonstrates how to use a machine learning model trained with  
**Google Teachable Machine** to classify images.  
The trained model is exported and loaded into the Google Colab environment to classify input images.

The code loads the model, preprocesses images to the required input format,  
performs prediction, and displays the predicted class along with the confidence score.

---

## Files Description

- `keras_model (1).h5`  
  The pre-trained Keras model exported from Google Teachable Machine.

- `labels.txt`  
  A text file containing class labels, each on a separate line, matching the model’s output order.

- `test.jpg`  
  The input image to classify (can be replaced with any other image).

---

## Methodology

1. **File Upload:**  
   Users upload the model, labels, and image files to Google Colab via the upload interface.

2. **Model Loading:**  
   The pre-trained Keras model is loaded without compiling for inference.

3. **Image Preprocessing:**  
   - Open the image and convert it to RGB format.  
   - Resize and crop the image to 224×224 pixels using Lanczos resampling to match the model’s expected input size.  
   - Normalize pixel values to the range [-1, 1] to align with the model’s training preprocessing.

4. **Prediction:**  
   The preprocessed image is passed to the model to get prediction probabilities for each class.

5. **Output:**  
   The class with the highest confidence score is selected, and both the class name and confidence percentage are printed.

---

## Usage Instructions

1. Upload the following files to your Google Colab session:  
   - `keras_model (1).h5`  
   - `labels.txt`  
   - `test.jpg` 

2. Run the provided Python script to perform classification.

3. Check the predicted class and confidence score in the output.

---


