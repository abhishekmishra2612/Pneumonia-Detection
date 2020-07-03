# Pneumonia-Detection using chest X-Ray image
## Business problem :
Given a chest X-Ray image of a person, predict whether this person surffering from pneumonia or not, if some how we are capable to detect of Pneumonia then we would help doctors to cure faster.
So we have built a deep learning model using tranfer learning technique to predict the presence of pneumonia by just scanning a chest X-Ray image.
### Source of Dataset : https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
## constraints :
It is not a low letency problem, but the cost of error is high. Model should give probability score of being pneumonia.
## Performance metrics :
Accuracy, area under ROC curve.
## Steps :
Collect the data from the kaggle and convert each image into numpy array.

I have used pretrained InceptionV3(Transfer Learning) model for extracting features from the chest X-Ray iamges, we got 2048 dimensional vector for each image.

Then built a Neural Network of some fully connected layers and the output layer has one sigmoid activation unit which gives the probability score of being pneumonia.

