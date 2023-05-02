Download Link: https://assignmentchef.com/product/solved-coen140-lab-7-neural-network
<br>
<strong>Problem: </strong>Build a two-layer neural network for image recognition with the fashion MNIST data set. The network has one hidden layer, and an output layer. The hidden layer has 512 nodes, and adopts the ReLU activation function; the output layer has 10 nodes, and adopts the softmax activation function to output the class probabilities. Use the “sparse_categorical_crossentropy” loss function, use ‘adam’ as the optimizer, and train your model for 5 epochs.

You can check this link regarding how to use the loss functions: https://keras.io/api/losses/probabilistic_losses/#sparse_categorical_crossentropy-function

The following code snippet is for you to start with: import tensorflow as tf from tensorflow import keras fashion_mnist = keras.datasets.fashion_mnist

(x_train, y_train), (x_test, y_test) = fashion_mnist.load_data() x_train, x_test = x_train / 255.0, x_test / 255.0

<strong>Include in the report : </strong>

<ol>

 <li>Select one image from each class to display as a gray-scale image.</li>

</ol>




<ol start="2">

 <li>Give the recognition accuracy rate of the whole test set, and show the confusion matrix.</li>

</ol>







<ol start="3">

 <li>Manually calculate the number of parameters in the neural network model. That is, the number of weight elements (include the bias terms). Show you work. Verify whether your results are the same as those given by model.summary().</li>

</ol>




Hint: calculate the number of parameters for each layer (hidden layer, and output layer), then sum them up.




<ol start="4">

 <li>Manually calculate the number of multiplications required to generate the hidden layer and the output layer. The weights have bias terms. You only need to consider the multiplications required to calculate the weighted sums. You don’t need to consider the multiplications involved in the softmax function. Show you work.</li>

</ol>

<strong>Demo/Explain to TA : </strong>

<ol>

 <li>How do you build the layers of the neural network?</li>

 <li>How do you specify the loss function, and the number of epochs?</li>

 <li>How do you calculate the number of parameters and the number of multiplications?</li>

</ol>


