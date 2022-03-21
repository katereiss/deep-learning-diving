The goal of this project is to train a neural network model to classify interesting dive photos from those that are not interesting.

The initial model used 125 interesting photos and 125 uninteresting photos. All photos are 224x224. The initial model was a keras Sequential model with an input layer, two dense laters with 3 units each and a RELU activation function, and a softmax activation in the output layer. 

Over 10 epochs, the categorical cross entropy loss was 0.6709, and the accuracy was 0.552. 

To improve upon this simple base model, I built a new model on top of the pretrained model MobileNet. This improved accuracy as shown below.

<img width="939" alt="Screen Shot 2022-03-21 at 3 14 46 PM" src="https://user-images.githubusercontent.com/84412675/159365971-193b10da-b03a-4b2d-b178-1cabb88b6b32.png">


The next steps will be focused on further improving the model. I will use 1000+ interesting and 1000+ uninteresting images in my dataset.

Some further actions to consider are tuning hyperparameters, altering the number of base layers taken from MobileNet, adding more images, and addressing overfitting. 
