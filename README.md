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

## Some predicted results :
This is the chest X-Ray image of a person who is normal(Ground truth) :
![NORMAL_7](https://user-images.githubusercontent.com/41646536/86440066-74d96580-bd27-11ea-8c3c-1baa570243a6.jpeg)  Predicted Score=0.068

This is the chest X-Ray image of a person who is suffering from Pneumonia(Ground truth):
![person1950_bacteria_4881](https://user-images.githubusercontent.com/41646536/86440583-5889f880-bd28-11ea-87ad-904de8523b1a.jpeg)  Predicted Score=0.997
