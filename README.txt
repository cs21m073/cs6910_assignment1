-->First of all load the fashion mnist data set and divide the dataset into train and test.
-->class FeedforwardNN contains all the operations to train the model.
-->In this we are using cross entropy as the loass function, sigmoid as the activation function and softmax as the output function.
-->class FeedforwardNN structure as follows:

class FeedforwardNN():
    def __init__(self, sizes, layers, epochs, l_rate): sizes contain number of nodes in each layer, layers contains the number of layer in the network, epochs contains the number of times we run the model, l_rate contains learning rate. We have two dictionary one is for weight and other is for bias that contains weights and bias for each layer      

    def sigmoid(self, x): return the sigmoid value of x
    
    def dsigmoid(self, x): return the derivative of sigmoid of x
    
    def ReLU(self, x): return the relu for x

    def dReLU(self,x): return the derivative of relu of x
    
    def softmax(self, x, derivative=False): return the softmax value of x if derivative is false else return the derivative of softmax of x

    def initialization(self): initializing all the weights and biases with random values

    def forward(self, x_train): taking x_train as input move forward from layer to layer and return the predicted output for x_train

    def backward(self, y_train, output): moving backward from output layer to input layer and calculating the changes in weights and biases at each layer and return the changes
    
    def update_parameters(self, changes_to_w, changes_to_b): making the changes in the original weight and bias at each layer    

    def compute_accuracy(self, x_val, y_val): computing the accuracy of the model and return the accuracy 

    def train(self, x_train, y_train, x_val, y_val): train the model on training set
 
 
          
            
            

