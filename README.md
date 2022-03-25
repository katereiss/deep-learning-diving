# Classifying Underwater Photos as Interesting or Not Interesting with Deep Learning

After a diving session, divers often have a large collection of underwater photos and videos. These photos and videos are often of varying quality due to motion, depth, and camera quality, among other factors. I wanted to create a machine learning classifier for my own dive photos to quickly sort through hundreds or even thousands of frames to find the interesting ones.

**Design and Data**

The first step was determining what an “interesting” photo is. I decided that clear images, recognizable subjects, and large marine life are important in interesting photos. 

I used CV2 to convert videos into series of images every 20 frames. My training dataset was slightly over 1,000 interesting and uninteresting photos for a total of around 2000 total training photos.

I chose to separate the testing data by video, so that similar frames from the same video did not affect the results. I used two videos for the testing data, one mostly interesting and one mostly not interesting. The total testing set was around 200 frames.

**Algorithms**

The final model used VGG16 as a base, with one trainable layer. I added a dense layer, a dropout layer with 0.25 dropout, and an output layer with a sigmoid activation function. On the testing set, the model performed with 91% accuracy, 99% precision, and 86% recall. 

**Tools**

- Keras
- Scikitlearn
- Matplotlib
- Numpy
- CV2
