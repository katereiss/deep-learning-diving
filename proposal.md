# Classifying Dive Photos As Interesting or Not Interesting with Deep Learning

**Project Proposal**

After a day of scuba diving, divers often have a large collection of underwater photos and videos. Often, due to the complications of underwater photography, some photos come out like the following:

![IMG_7835](https://user-images.githubusercontent.com/84412675/158687671-22d240d1-2bf1-4417-bacc-718e50d9d809.jpg)




The goal of this project is to train a neural network model to classify interesting dive photos from those that are not interesting. While “interesting” is subjective, some indications of interesting photos are clear images and recognizable subjects.

![IMG_6872](https://user-images.githubusercontent.com/84412675/158687695-27e1829c-96fc-4e72-b7c6-96c1ed10f97d.jpg)


Dive images and videos will be my own, and may be supplemented with other divers’ media if I don’t have enough. Videos will be split into series of images. Images will be formatted so that all images are of equal size. 

An initial MVP will be trained on at least 100 interesting and 100 uninteresting images. An initial model will be a deep learning model, as the complexity of image data justifies starting off with a complex model. The final model will include over 1000 interesting and 1000 uninteresting images. 

The metric used to determine model performance will be F-beta with a beta score of 2, as both precision and recall are prioritized with an emphasis on recall. Avoiding false negatives, when an interesting photo is classified as uninteresting, is prioritized over avoiding false positives. 

Algorithms to explore are convolutional neural networks and transfer learning. Cloud computing resources may be necessary for the model containing all of the data. 



