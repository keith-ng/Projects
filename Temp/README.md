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
Unedited | - | ✓ | ✓ | ✓


### Model Selection:

Selection Criteria:
- Applicability:
	- Since the application is undefined, we seek to implement a model that performs well with a small dataset as it will allow application to a wider range of cases
- Feasibility:
	- With access to only a local terminal to test the model, a large and complex dataset may prove to be unfeasible
- Model Accuracy:
	- The selected model however, has to achieve a respectable accuracy as an inaccurate model serves no purpose.


Primary Criteria:
-  Model Accuracy 
	- PiT: 92.07
	- PSTA: 91.5

### Model Comparison:

Traditional Trackers:
- FairMOT
	-
- DeepSORT
	-


### Files used:

- train.csv -- data containing all of the training data.




  

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

