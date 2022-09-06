# Detection Techinques

## Noraml CNNs
One of the methods is to train a CNN like VGG or ResNet on datset having both the classifiaction and bounding boxes of the object and the loss function becomes hybrid between the classification problem and the regression problem of the position of hte bounding boxes, the main disadvantage of this method is the the lack of the dataset and it's hard to gneralise the model on different secnarios.

## Sliding Windows Approach
This approach from its name slides a window over the picture and classifies the window each time, if a certain class probability exceeds a certain threshold then a bounding box is placed, most probably their will be lts of overlapping bounding boxes so algorithms like non-max suppression are used.
### Main Disadavantages
- Needs high computational power as each part of the image is classified at least one time.
- The windows size is a hyperparameter and in the same picture we may need to slide different windows wiith different sizes.
### Note
There is impleemnation of CNNs thaat embed the sliding window approach within the network itself which makes the process more convenient.






