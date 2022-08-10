I have included several pretrained models. The best two I generated are marked BestWorkingModel and SecondWorkingModel.
The CanBottleTesting directory contains images that were not used in the training and validation process of the pretrained models.
Here is a video demo of the SecondWorkingModel: 
https://www.youtube.com/watch?v=6tCCQ93_S1s

There is an evolution to my naming convention, but the files I have included almost entirly use 3x3 kernals. 
Each convolutional layer has a ReLu activation. 
The first  dense layer also has a ReLu activation, as well as a varying filter size. Any additional dense layers didn't have ReLu.
Filter size of the convolutional layers is denoted by an integer value. 

2x64-32-16-64d-8e
This would denote two 64 filter layers, followed by a 32 and 16 filter layer, all with kernal size 3. 
64 filters dense layer, with 8 epochs.

Models denoted with R such as 
2x64-32-16-64d-8eR1 are trained on a different seed of validation split.
-softmax denotes the output is normalized to certainty percentages.