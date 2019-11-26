
# 🄳🄴🄴🄿 🄻🄴🄰🅁🄽🄸🄽🄶  🄶🄻🄾🅂🅂🄰🅁🅈 (>‿◠)✌


---

- batch-size

  the number of training examples in one forward/backward pass. The higher the batch size, the more memory space you'll need.

- iterations

  An *iteration* describes the number of times a *batch* of data passed through the algorithm. In the case of neural networks, that means the *forward pass* and *backward pass*. So, every time you pass a batch of data through the NN, you completed an *iteration*.

- epochs

  An *epoch* describes the number of times the algorithm sees the *entire* data set. So, each time the algorithm has seen all samples in the data-set, an epoch has completed.

  ---

- validation-set

  this data set is used to minimise over-fitting. You're not adjusting the weights of the network with this data set, you're just verifying that any increase in accuracy over the training data set actually yields an increase in accuracy over a data set that has not been shown to the network before, or at least the network hasn't trained on it (i.e, validation data set). If the accuracy over the training data set increases, but the accuracy over the validation data set stays the same or decreases, then you're over-fitting your neural network and you should stop training.

- training-set

   this data set is used to adjust the weights on the neural network.

- test-set

  this data set is used only for testing the final solution in order to confirm the actual predictive power of the network.

  ---
- flops

  One way to get an idea of the speed of your model is to simply count how many computations it does. We typically count this as [FLOPS](https://en.wikipedia.org/wiki/FLOPS), floating point operations per second. 


- confusion matrix

- Mean Average Precission - (mAP)

- precission-recall

- loss function

- mAP curve

- parameters

- tensors

- checkpoint

- backbone of network

- res-net

- mobile-net

- roi-extractor

- feature maps

- FCN network

- FPN

- loss function

- Intersection over Union (IoU)

- ROI pooling, align, warping



---

> If you wish to contribute you can do it by forking this repo. ✍(◔◡◔)
