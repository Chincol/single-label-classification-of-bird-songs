# single-label-classification-of-bird-songs
This is a system developed to classify single label bird song present in an audio wave file. The classificartion is done using Deep Neural Network which is first trained by using providing training dataset and then furter classify the files using trained network.


Files are to be used in the order they are mentioned in this readme file.
Files are to be run on the same system as the class labels order may change with system.

# process.py
  This file is for generating context windows from training data and merging all training data into a single file.
  This includes all classes.

# pretrain.py / dnn.py or any such file
  The training file created from process.py is input to this file.
  This file is for training the network one can change various parameters.
  Each such subsequent file is to be run in the order of number mentioned in their file names.
  Each subsequent file trains one additional layer of the neural network.
  The output of this each such file is a parameters.pkl file which stores the parameters of the network learnt.

# load_dnn.py
  This file is used for testing the trained network.
  The input to this file is the parameters.pkl file from the obtained from training.
  The model is then loaded using the weights in the .pkl file.
  The file then calculates the accuracy and the confusion matrix.
  
Code written by : Deep Chakraborty
