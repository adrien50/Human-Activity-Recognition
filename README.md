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
