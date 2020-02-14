# Recognising-Handwritten-Digits

Handwritten Digit Recognistion using CNN. The training data is imported from MNIST dataset. The cnn model is made using keras library.
Since, the input shape is in the (6000,28,28). We need to reshape the training input data and the test input data in form of (6000,28,28,1).
So that the data can fit into the neural net. 
Since y_test and y_train ranges from (0 to 9). It is transformed into categorical data.
CNN is made using the keras library.
Sequential model is used to form CNN using layer by layer.
Then convolution on image matrix is done by 3x3 filter matrix and maxpooling is applied with a dropout of 0.25 (It can be tuned for better results.)
After maxpooling, the layer is flattned. So that, it can be used as input in neural network as 1-D vector.
The rest of thr hidden layers is made by dense function.
Model is compiled using 100 epochs and batch size of 128.( It can also be tuned for better results.)

Test loss: 0.0539406917522289
Test accuracy: 0.9926000237464905

Tikinter model is used for testing handwriting digits.
