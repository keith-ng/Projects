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
- The iLIDs dataset only consists of 300 unique individuals and may be too small to create a robust model as a result of underfitting.

### Model Selection:

Selection Criteria:
- Applicability:
	- Since the application is undefined, we seek to implement a flexible model that performs well in as many situations as possible.
		- To achieve this, the model should return a respectable score with the iLIDs dataset as there may be cases where the model has to be retrained with new data and we have some level of assurance that it can perform well with small datasets
- Feasibility:
	- With access to only a local terminal to test the model, a large and complex dataset may prove to be unfeasible to train and test.
- Model Accuracy:
	- The selected model ideally will perform well with different datasets as it will increase the likelihood of it performing well in new unseen data.
	- The selected model PiT obtained the highest scores for 4 metrics with the iLIDS-VID dataset and top 3 for 4 metrics with the MARS dataset

### Model Evaluation:

Given the focus of projects on security and retail, we test the model on a video with shoplifting occurence to see if we can re-identify individuals captured by different cameras in a gas station.  

### Acknowledgement:This repository is built upon the repository TranReID.


### Citation:
@ARTICLE{9714137,
  author={Zang, Xianghao and Li, Ge and Gao, Wei},
  journal={IEEE Transactions on Industrial Informatics}, 
  title={Multidirection and Multiscale Pyramid in Transformer for Video-Based Pedestrian Retrieval}, 
  year={2022},
  volume={18},
  number={12},
  pages={8776-8785},
  doi={10.1109/TII.2022.3151766}
}

### Project Status:
- Plans to refine the model further are subjected to availability.
