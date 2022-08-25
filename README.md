# Digit Recognition w/ CNN from Scratch

## Summary
The contained python files provide a framework to implement and train a convolutional neural network that recognizes hand-written digits. The framework is written from scratch (no TensorFlow, only NumPy). I incorporated gradient descent, dropout regularization, adam optimization into the framework. Please note that vectorization is only implemented on the dense layers, so training is slow. My own implementation achieved a roughly 98% dev set accuracy rate. 

## Structure
main.py -- where the main method is stored and where training/testing is called. 
cnn.py -- the network module containing the class DenseLayer, ConvLayer, PoolLayer, FlattenLayer, responsible for forward and backward propagation of the network
networkio.py -- stores and reads network and training information in files via pickle
training.csv -- the dataset
network.pickle -- the pickle file that can be read through networkio.py, stores the network I trained myself.
cost_map.png -- image generated by matplotlib that maps the movement of cost function value during training

## Data source
The dataset (training.csv after unzipping training.zip) comes from: https://www.kaggle.com/c/digit-recognizer

## Example Network
training set accuracy:  
accuracy: 39707 out of 40000 times (0.992675)  
dev set accuracy:   
accuracy: 983 out of 1000 times (0.983)  
test set accuracy:  
accuracy: 980 out of 1000 times (0.98)  
