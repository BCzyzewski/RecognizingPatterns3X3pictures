## Recognizing patterns on 3 X 3 pixel pictures using Neural Networks

##### Overview of the repository
This repository contains a main file "Recognize Patterns.ipynb" where we can find a Machine Learning algorithm used for recognizing patterns on a black and white 9-pixel picture.

##### What kind of patterns will be recognized?
There are 4 main patterns that the algorithm is recognizing.

The first one is the <b>solid pattern</b>:
<center><img src="Patterns_Examples\Solid pattern.png"></center>
As we can see all of the 9 pixels of the image are solid black. That is the only configuration of pixels possible for this pattern. This one is the easiest to recognize.

The next one is the <b>vertical pattern</b>. Please look at the example below.
<center><img src="Patterns_Examples\Vertical pattern.png"></center>
This pattern occurs when any of the 3 possible vertical lines of pixels are black. Because of this there 3 different images that can have this pattern.

The third one is <b>diagonal</b>. There is an example below.
<center><img src="Patterns_Examples\Diagonal pattern.png"></center>
This one occurs when 3 pixels on the diagonal line are black. There are two 2 possible different pictures that can have this pattern.

The last one is the <b>horizontal</b> pattern. Please look at the example below.
<center><img src="Patterns_Examples\Horizontal pattern.png"></center>
We can see this pattern, when any of the 3 horizontal lines are filled with black pixels. There are 3 possible images like this.

##### Which model was used to recognize patterns?

A standard neural network was used built by the keras API from the TensorFlow framework. There are 4 different models with various number of hidden layers and activation functions.

Dataset for training the network has 4000 images and the test set has 1000 images.

##### Results
Three out of four models have achieved accuracy on the validation set equal to 1. This result is very good, as we were able to build models that 100% of a time were able to predict the right pattern. The only model that was lacking in accuracy is the last one with random weights. This was to be expected as the weights should be optimized during data fitting.