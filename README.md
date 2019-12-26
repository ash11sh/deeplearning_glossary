
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

#### Calculate AP

For each class:

First, your neural net **detection-results** are sorted by decreasing confidence and are assigned to **ground-truth objects**. We have "a match" when they share the **same label and an IoU >= 0.5** (Intersection over Union greater than 50%). This "match" is considered a true positive if that ground-truth object has not been already used (to avoid multiple detections of the same object). 
  
  <img src="https://user-images.githubusercontent.com/15831541/37725175-45b9e1a6-2d2a-11e8-8c15-2fb4d716ca9a.png" width="25%" height="25%" />

​	Using this criterium, we calculate the precision/recall curve. E.g:

​	<img src="https://user-images.githubusercontent.com/15831541/43008995-64dd53ce-8c34-11e8-8a2c-4567b1311910.png" width="45%" height="45%" />

Then we compute a version of the measured precision/recall curve with 	**precision monotonically decreasing** (shown in light red), by setting 	the precision for recall `r` to the maximum precision obtained for any recall `r' > r`.

Finally, we compute the AP as the **area under this curve** (shown in light blue) by numerical   integration.
No approximation is involved since the curve is piecewise constant.

#### Calculate mAP

​	We calculate the mean of all the AP's, resulting in an mAP value from 0 to 100%. 

> you can use this [code](https://github.com/Cartucho/mAP) to evaluate your object detection model

E.g:

<img src="https://user-images.githubusercontent.com/15831541/38933241-5f9556ae-4310-11e8-9d47-cb205f9b103b.png" width="35%" height="35%" />

<img src="https://user-images.githubusercontent.com/15831541/38933180-366b6fca-4310-11e8-99b9-17ad4b159b86.png" width="35%" height="35%"  />

---

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
