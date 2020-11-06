I tried different layers of convolution, pooling and dense.
I noticed that by increasing the number of convolutional and pooling layers accurracy increased.
By adding a dropout results improved in a somewhat linear fashion as opposed to 
barely improving between different epochs without dropout which shows the effect of overfitting.
After flattening, adding dense layers was tricky because adding too many was counterproductive and was not optimal.
All layers had Relu activation except for the output layer that had softmax as we have several exclusively different classes.
Loss function was set to categorical crossentropy for the same reason: we have 43 classes as output.
