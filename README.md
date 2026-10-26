In this project, with the use of transfer learning, 
we train a convolutional neural network for the task of detecting the presence of pneumonia on the rentgen photos of lungs.

This project can be separated into several parts.

First one consists of:
 - loading the data,
 - augmenting them into adequate form,
 - separating them into train, test and val sets.

Second part consists of finding optimal sizes and parameters for feed-forward layers in the final network with the use of Optuna, 
and creation of said network with the use of transfer-learning mechanism based on the ResNet50 network.

Third and final part contain the training loop with the early stop condition, that checks if the validation loss decreased in the last 5 epochs,
if not the training loop is interrupted and restarted with the last saved network version.
