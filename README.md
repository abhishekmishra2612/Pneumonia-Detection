# Pneumonia-Detection using chest X-Ray image
## Business problem :
Given a chest X-Ray image of a person, predict whether this person surffering from pneumonia or not, if some how we are capable to detect of Pneumonia then we would help doctors to cure faster.
So we have built a deep learning model using tranfer learning technique to predict the presence of pneumonia by just scanning a chest X-Ray image.
## Source of Dataset : https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
## constraints :
It is not a low letency problem, but the cost of error is high. Model should give probability score of being pneumonia.
## Performance metrics :
Accuracy, area under ROC curve.
## Steps :
To build this project i used InceptionV3(Transfer Learning) for feature extraction and apply fully connected dense layers network to get final output(Probability score of having PNEUMONIA).
The output(probability score) gives the possibility of a person having PNEUMONIA .
The dataset i got from kaggle.com
Link of dataset 
