# Siamese-Networks

Designed and implemented (using Pytorch) a CNN architecture which as input takes two images of digits from MNIST dataset and outputs 1 if both images correspond to the same digit and 0 otherwise using the concept of Siamese Networks.

I have used 10% of MNIST training data set as the training data set and only 10% of MNIST test data set as test
data set.

The network takes as input a 4-dimensional tensor: (batch size, plane count - each plane corresponds to a different input digit image, image height, image width). 

Loss function:
For calculating loss I have used contrastive loss. It is a distance-based Loss function. It tries to ensure that
semantically similar examples are embedded close together

Training Loss:
The training loss decreases eventually with the increase in number of iterations

Test Loss:
The test loss also decreases for our test data starting from 3.5 to 2.3 in 30 epochs.
