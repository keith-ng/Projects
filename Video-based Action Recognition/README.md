## Video-Based Person Re-Identification

### Project Description:

The goal of this project is to implement a video-based Person Re-Identification algorithm on a single camera. We assess and select existing publicly-available algorithms [here](https://paperswithcode.com/task/video-based-person-re-identification) and identify their relevance (if any) for this case.

Final model selected is user deropty's PiT model. Instructions to implement the model can be found on his [GitHub](https://github.com/deropty/PiT).

### Datasets Summary:

Dataset | MARS | DukeMTMC | iLIDS | Airport 
--- | --- | --- | --- |--- 
ids | 1261 | 2700 | 300 | 9651 
images | - | 2000000 | - | 39902
tracklets | 20478 | - | 600 | -
bboxes | 1191003 | - | 43800 | -
distractors | 3248 | 0 | 0 | 0
cameras_num | 6 | 8 | 2 | 6

**Datasets Comparison**
Dataset | MARS | DukeMTMC | iLIDS | Airport 
--- | --- | --- | --- |--- 
Sample Size | ✓✓ | ✓✓ | ✓ | ✓✓✓
Image Variations | ✓✓ | ✓✓✓ | ✓ | ✓✓
Raw | - | ✓ | ✓ | ✓

To create a robust model, we seek to train the model with a vast dataset. 
- Although 'Airport' is the largest dataset, it has the least number of independent studies and exposure which does not inspire the most confidence in the data's integrity.
- The DukeMTMC dataset is the second largest dataset. However, it has since been retracted due to external factors, thus we refrain from using it as well.
- The **MARS dataset** is relatively big and widely used in numerous papers & studies, and it seems to be the most appropriate dataset so far.
- The iLIDs dataset only consists of 300 unique individuals and may be too small to create a robust model due to underfitting.

### Model Selection:

Selection Criteria:
- Applicability:
	- Since the application is undefined, we seek to implement a model that performs well in as many situations as possible.
	- The model should return a respectable score with the iLIDs dataset as there may be cases where the model has to be retrained with new data and we have some level of assurance that it can perform well with small datasets
- Feasibility:
	- With access to only a local terminal to test the model, a large and complex dataset may prove to be unfeasible to test.
- Model Accuracy:
	- The selected model ideally will perform well with different datasets as it will increase the likelihood of it performing well in new unseen data.

  

### Files used:

- train.csv -- data containing all of the training data.

### Codebook / Data Dictionary:


  

### Credits:

### Project Status:
- Plans to refine the model further are subjected to availability.
