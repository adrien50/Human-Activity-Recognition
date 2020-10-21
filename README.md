# What is Human Activity Recognition

According to [machinelearningmastery](https://machinelearningmastery.com/deep-learning-models-for-human-activity-recognition/), it involves predicting the movement of a person based on sensor data and traditionally involves deep domain expertise and methods from signal processing to correctly engineer features from the raw data in order to fit a machine learning model.Recently, deep learning methods such as convolutional neural networks and recurrent neural networks have shown capable and even achieve state-of-the-art results by automatically learning features from the raw sensor data. The difficulty is that this feature engineering requires strong expertise in the field. Recently, deep learning methods such as recurrent neural networks like as LSTMs and variations that make use of one-dimensional convolutional neural networks or CNNs have been shown to provide state-of-the-art results on challenging activity recognition tasks with little or no data feature engineering, instead using feature learning on raw data.

# LSTMs for Human Activity Recognition

Human Activity Recognition (HAR) using smartphones dataset and an LSTM RNN. Classifying the type of movement amongst six categories:
* WALKING,
* WALKING_UPSTAIRS,
* WALKING_DOWNSTAIRS,
* SITTING,
* STANDING,
* LAYING.

Compared to a classical approach, using a Recurrent Neural Networks (RNN) with Long Short-Term Memory cells (LSTMs) require no or almost no feature engineering. Data can be fed directly into the neural network who acts like a black box, modeling the problem correctly. 

# What is an RNN?

According to [kdnuggets](https://www.kdnuggets.com/2020/07/pytorch-lstm-text-generation-tutorial.html)RNNs are neural networks that are good with sequential data. It can be video, audio, text, stock market time series or even a single image cut into a sequence of its parts. Standard neural networks (convolutional or vanilla) have one major shortcoming when compared to RNNs - they cannot reason about previous inputs to inform later ones. You cannot solve some machine learning problems without some kind of memory of past inputs. For example, you might run into a problem when you have some video frames of a ball moving and want to predict the direction of the ball. The way a standard neural network sees the problem is: you have a ball in one image and then you have a ball in another image. It does not have a mechanism for connecting these two images as a sequence. Standard neural networks cannot connect two separate images of the ball to the concept of “the ball is moving.” All it sees is that there is a ball in the image #1 and that there's a ball in the image #2, but network outputs are separate.For more understanding of RNN,read [here](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)

# What is LSTM ?

LSTM is a variant of RNN used in deep learning. You can use LSTMs if you are working on sequences of data. Here are the most straightforward use-cases for LSTM networks you might be familiar with:
* Time series forecasting (for example, stock prediction)
* Text generation
* Video classification
* Music generation
* Anomaly detection
For more understanding of LSTM, you can read [here](http://colah.github.io/posts/2015-08-Understanding-LSTMs) 

# Project Statement

The project aims to detect whether the person is running or 
walking based on deep neural network and sensor data collected 
from iOS device.Currently, the dataset contains a single file 
which represents 88588 sensor data samples collected from 
accelerometer and gyroscope from iPhone 5c in 10 seconds interval 
and ~5.4/second frequency. This data is represented by following 
columns (each column contains sensor data for one of the sensor's
 axes):

* acceleration_x
* acceleration_y
* acceleration_z
* gyro_x
* gyro_y
* gyro_z
* There is an activity type represented by "activity" column which 
acts as label and reflects following activities:

* "0": walking
* "1": running
Apart of that, the dataset contains "wrist" column which 
represents the wrist where the device was placed to collect a
 sample on:

* "0": left wrist
* "1": right wrist
Additionally, the dataset contains "date", "time" and "username" 
columns which provide information about the exact date, time and 
user which collected these measurements.

