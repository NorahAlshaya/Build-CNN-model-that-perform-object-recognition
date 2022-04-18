# Build-CNN-model-that-perform-object-recognition
We used the CIFAR-10 dataset that consists of 60000 32x32 color images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.  


The CNN model consists of 3 sets each containing 2 convolutional layers followed by a pooling layer. Initially, Providing the input image into the 1st set by applying the filters with stride, and padding. Perform convolution on the image and apply the ReLu as an activation function to the matrix. After that, performing pooling to reduce the dimensionality size. Add 2 more sets and perform the previous steps. Then, flatten the output and feed it into a fully connected layer (FC layer). Finally, output the class using the SoftMax activation function and classifies images. 

The reason that we apply two consecutive convolutional layers followed by a pooling layer instead of a convolutional layer then pooling layer is to build up better representations of the data without quickly losing all of spatial information, because pooling decreases the dimensions of your data exponentially. 
