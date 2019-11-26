
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

  A **confusion matrix**, in predictive analytics, is a two-by-two table that tells us the rate of false positives, false negatives, true positives and true negatives for a test or predictor. We can make a confusion matrix if we know both the predicted values and the true values for a sample set.

  In machine learning and statistical classification, a confusion matrix is a table in which predictions are represented in     columns and actual status is represented by rows. Sometimes this is reversed, with actual instances in rows and predictions in  columns. The table is an extension of the confusion matrix in predictive analytics, and makes it easy to see whether mislabelling has occurred and whether the predictions are more or less correct.

  <p align="center"><img src="https://live.staticflickr.com/65535/49127153233_d8af9a98ce_o_d.png" width="600"></p>
  

   
   Here **a** is the number of true negatives, and **d** the number of true positives. **b** is the number of false positives, and   **c** is the number of false negatives. 



    - The **accuracy** of the prediction or test is defined as (a + d)/(a + c + d + e).
    - The **true positive rate** is given by d/(c + d), and is also called the recall. It tells us what proportion of positive cases were correctly identified. 
    - The **false positive rate**, or proportion of negative cases (incorrectly) identified as positive, is given by b/(a + b).
    - The **true negative rate** is a/(a + b), and represents the proportion of negative cases that were correctly identified. 
    - The **false negative rate** is c/(c + d), and tells us what proportion of positive cases were incorrectly labeled as negative.
    - The proportion of the instances we correctly labeled as positive  (per total positive prediction) is given by d/(b + d) and is called the **precision**. 

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
