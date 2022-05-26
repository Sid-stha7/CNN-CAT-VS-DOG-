# CNN-CAT-VS-DOG-
Binary Classification of cat and dog class using Convolution Neural Network (CNN). This project is able to classify the cat and dog image with accuracy of 80%.

# Model Summary
There are 6 layers in this layer with 2,51,00,046 total parameters i.e.,

* Input layer,
* Convolutional 2D layer,
* Max Pooling 2D layer,
* Flattern Layer,
* Dense Layer and
* Output layer

![image](https://user-images.githubusercontent.com/106294475/170423064-e3fa80bd-4393-400b-bbbe-ba938aa08f91.png)

The hyper parameters that are used in order to develop this model are

* batch size,
* target size,
* class mode,
* epoch, steps
* epoch,
* validation steps

Among above hyper-parameters 6 are trainable hyper-parameters of this model.

# Training model: 
In the model “Categorical Crossentropy” was used as loss Function and the optimization algorithm that
is used in this model is “ADAM” and the model was trained for 20 epochs.

![image](https://user-images.githubusercontent.com/106294475/170423491-146abde5-b086-453c-b283-c8bcc2f0fb1a.png)

# Categorical Crossentropy as Loss Function:

![image](https://user-images.githubusercontent.com/106294475/170423528-26ecc473-a2f3-4321-b710-4767fb34a0ea.png)

# Epoch Initialization:

![image](https://user-images.githubusercontent.com/106294475/170423563-2d2512dc-e80e-41a6-8f07-61f3431a2f36.png)
![image](https://user-images.githubusercontent.com/106294475/170423620-61538686-a82f-48bb-9abc-d3c937ea584c.png)
![image](https://user-images.githubusercontent.com/106294475/170423674-ffbcb6f2-1f69-4b2b-940d-e8f9c89bceb7.png)

# Findings:
For evaluation of our model, we have used confusion matrix and calculated precision, recall, f1score
accuracy, macro average and weighted average. Confusion matrix is one of the widely used evaluation
metrics of any classification problems, it shows the value of actual and predicted out comes. The
confusion matrix that was being calculated was of 2 class i.e., dog and cat. From the confusion matrix
the report we are able to generate is as follow:

![image](https://user-images.githubusercontent.com/106294475/170423845-3f69817b-3877-464e-b7e5-2bd41c6ece33.png)


# True Positive count (TP): 
The true positive count that our model was able to generate is 391. Which
means that out of 2023 image data of dogs and cat the model was able to predict 391 images of cat as
cat class correctly.
# True Negative count (TN): 
The true negative count was 601 which it the count for non-cat prediction.
The model was able to identify 601 image data of dogs correctly out of 2023 total data.
# False negative count (FN): 
The false negative count was 620 of the models which means the model
falsely predicted 620 cat images as dog.
# False positive count (FP): 
The model predicted falsely 411 images as a cat although the images were
from the dog class.

<h3>And now as per our classification report following are the metrics, we were able to generate
From confusion matrix:</h3>

# Precision: 
The ratio of properly categorized data is a measure of an algorithm's precision. The rate in
which our model predicts all the test images as cat and all the test images as dog is 0.49.
# Recall: 
It is the ratio of total correctly prediction of true upon total positive values. In out case the rate in
which model was able to classify cat correctly from total positive value is 0.39 and the rate in which
model was able to classify dog correctly from total positive value is 0.59.
# F1-score: 
It is the harmonic mean of precision and recall. It is maximum when Precision=Recall. The f1-
score of our model was 0.43 for cat as true and 0.54 for dog as true.
<h3>The macro average and weighted average of the model was 0.49.</h3>

![image](https://user-images.githubusercontent.com/106294475/170424421-f393a693-b24f-4894-96fb-ec7ca3a32ccf.png)

# Result

<h3> After the model was successfully trained. For test 1 we had given input of a file which is cat picture and
after it went in out prediction model. The model classified the picture as cat. The input file and result are
shown below </h3>

![image](https://user-images.githubusercontent.com/106294475/170424550-3d6f231e-0e46-4ab8-91d8-3f6054de1c0b.png)

<h3>For test 2 we had given input of a file which is a dog picture and after it went in out prediction model. </h3>

![image](https://user-images.githubusercontent.com/106294475/170424668-2054a896-a370-490c-89c6-5ce96b97ce6c.png)

<h3>The model classified the picture as dog. The input file and result are shown below: </h3>

![image](https://user-images.githubusercontent.com/106294475/170424738-28c2c120-47f9-4210-a54a-4b58b58d3f11.png)

# Recommendation:
In future the model shall not be made for only of 2 classes, it will be escalated into more than 2 classes.
The accuracy of the model can be increased by properly tuning the hyper parameters. The model will be
evaluated on different algorithms and activation functions as well. In order to make the model more
accurate it will be trained for more epochs.
