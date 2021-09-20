# Overview
-----
This project is built upon the MLEnd dataset which is comprised of 20,000 audio samples of numbers provided by students at Queen Mary's University. 

This notebook is split into 2 primary sections; a basic solution and an advanced section, in which models are built and tested to achieve different outcomes. This notebook was intended to run on Google Colab. 

A high level summary of the two solutions can be seen below: 

1.   **Basic Solution**:

 A model is created to identify the intonation of a numeral contained in an audio file. Possible intonations are neutral, bored, excited or phrased as a question. The model will use hand-crafted features (primarily available through `sk-learn`) to create decision boundaries for 3 different types of classifiers; SVM, Gaussian Naive Bayes and K-nearest neighbours. Each classifier is evaluated using a validation dataset and different features are combined to try to maximise the accuracy of predictions.
 
 An accuracy of c. 67% is achieved for correctly identifying the intonation of the spoken numerals from a vaidation dataset. 

2.   **Advanced Solution**: 

 A model created to identify the numeral spoken, using a convolutional neural network to identify features from an mfcc spectogram. Once the model has been trained a potential real-world use case is discussed and demonstrated wherein the model is used to identify mobile numbers read out in an Interactive Voice Response (IVR) system.
 
 An accuracy of 77% is achieved for correctly identifying the spoken numeral using a convolutional neural network with 3 convolutional layers after 30 epochs of training. 
