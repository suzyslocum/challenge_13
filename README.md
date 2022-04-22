# Predicting Startup Success for a Venture Capital(VC) Firm

*Module 13 Challenge Assignment *

---

## Overview of the Analysis
---
  In order to predict whether or not a startup will be successful, we use a binary classifier model. We then optimize the model and compare the accuracy of the different models that were created and trained.

  First the data was seperated in to "labels" and "features". The label is the variable we are interested in making predictions about, in this case, the success of startups that are being funded by this VC firm. The features are the remianing categories of information in the dataset. A binary classifier model was created using the TensorFlow and SciKit-Learn libraries to make predictions on new data about startups the VC firm may potentially fund. It was tested on historical data so that its accuracy may be assessed. The model was then optimized by removing features that may confuse the model, adding more hidden layers, and changing the number of epochs. These changed were made seperately. The new models then made predictions, and the accuracy of those predictions was assessed. 


## Results
---

* Original Model - all features used, two hidden layers used, average of input & output nodes used for first hidden layer, average of nodes of first hidden layer & output layer used for second hidden layer, relu used for activation of hidden layers, sigmoid used for activation of output layer, 50 eopchs used:
  * The model's accuracy was assessed to be 73%
  * The model's loss was assessed to be 55%.
    

* Alternative Model 1 - "Special Considerations" and "Status" columns removed, but otherwise the same as the original model:
  * The model's accuracy was assessed to be 73%
  * The model's loss was assessed to be 56%.


* Alternative Model 2 - Added two additional hidden layers for a total of four hidden layers, but otherwise the same as the original model:
  * The model's accuracy was assessed to be 73%
  * The model's loss was assessed to be 56%.


* Alternative Model 3 - 200 epochs used, but otherwise the same as the original model:
  * The model's accuracy was assessed to be 73%
  * The model's loss was assessed to be 57%.
    

## Summary
---
Given the lack of improvement in accuracy and loss, I would not recommend that any of the alternative models be used. The original model itself is also not very accurate at only 73%. I would reccommend that more alterations be made until improvement is found, or that an entirely different type of model be used for these predictions given the potential loss of investment capital. 


![original_model_summary](/Images/original_model_summary.jpg)
![original model_accuracy](/Images/original_model_accuracy.jpg)


---

## Technologies

The application is written in Python using Pandas
The following packages are used:

Pandas - to write and run the program [Pandas documentation](https://pandas.pydata.org/docs/)

Pathlib - to create file paths [Pathlib documentation](https://docs.python.org/3/library/pathlib.html)

TensorFlow - to generate deep learning models - [TensorFlow documentation](https://www.tensorflow.org/guide)

SciKit-Learn - to train models, encode data, and scale data [SciKit Learn documentation](https://scikit-learn.org/0.21/documentation.html)


---

## Installation Guide

Install the Pandas package using the following command: 'import pandas as pd'

Install the Pathlib module using the following command: 'from pathlib import Path'

Install the TensorFlow libraries using the following commands: 'import tensorflow as tf', 'from tensorflow.keras.layers import Dense','from tensorflow.keras.models import Sequential'

Install the SciKit-Learn metrics libraries using the following commands: 'from sklearn.model_selection import train_test_split', 'from sklearn.preprocessing import StandardScaler,OneHotEncoder


--- 

## Usage

To run this program, clone the repository onto your computer, navigate to its source folder in your terminal and launch it using the command 'jupyter lab' then either run the entire program at once, or run the cells individually (in order) as you move through the file.

---

## Contributors
Susannah Slocum 
suzyslocum@gmail.com

---

## License

None
