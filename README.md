# Modified-ResNet-for-CIFAR-10-Classification-with-Under-5-Million-Parameters

**Goal**

In this mini-project we were tasked with coming up with a modified residual
network (ResNet) architecture with the highest test accuracy on the CIFAR10 image classification dataset, under the constraint that your model has no
more than 5 million parameters.\\

**Details**

Recall that a residual network (ResNet) architecture is any convolutional network with skipped connections. Here is a picture of ResNet-18:
The key component in ResNet models is a residual block that implements: 
ReLU(S(x) + F(x)) where S(x) refers to the skipped connection and F(x) is a block that implements conv -> BN -> relu -> conv -> BN; here, “BN” stands for batch normalization. Chaining such blocks serially gives a deep ResNet.

Hyperparameters (design variables) in such architectures include:
• Ci
, the number of channels in the ith layer.
• Fi
, the filter size in the ith layer
• Ki
, the kernel size in the ith skip connection
• P, the pool size in the average pool layer,
etc.
