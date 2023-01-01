
# Building and Road Segmentation from Aerial Images using EffUNet

In city, information about urban objects such as water supply, railway lines, power lines, buildings, roads, etc., is necessary for city planning. In particular, information about the spread of these objects, locations and capacity is needed for the policymakers to make impactful decisions. This thesis aims to segment the building and roads from the aerial image captured by the satellites and UAVs. Many different architectures have been proposed for the semantic segmentation task and UNet being one of them. In this thesis, we propose a novel architecture based on Google’s newly proposed EfficientNetV2 as an encoder for feature extraction with UNet decoder for constructing the segmentation map. Using this approach we achieved a benchmark score for the Massachusetts Building and Road dataset with an mIOU of 0.8365 and 0.9153 respectively.


## Tech Stack

**Libraries:** PyTorch, Numpy, Matplotlib, SMP 



## Results

### Evaluation of different models for building dataset

| Model | mIOU | Dice Loss | Precision | Recall | F1 Score | Accuracy |
| :---: | :---: |  :---: |  :---: |  :---: |  :---: |  :---: |  
|V2S+UNet|0.8159|0.1054|0.8746|0.9220|0.8977|0.8997|
|V2M+UNet|0.8293|0.0977|0.8821|0.9316|0.9062|0.9080|
|B7+UNet|0.8359|0.0934|0.8863|0.9352|0.9101|0.9119|
|V2L+UNet|0.8365|0.0925|0.8865|0.9356|0.9104|0.9122|

### Evaluation of different models for road dataset

| Model | mIOU | Dice Loss | Precision | Recall | F1 Score | Accuracy |
| :---: | :---: |  :---: |  :---: |  :---: |  :---: |  :---: |  
|V2S+UNet|0.9139|0.0453|0.9321|0.9786|0.9548|0.9558|
|V2M+UNet|0.9140|0.0475|0.9323|0.9786|0.9549|0.9559|
|V2L+UNet|0.9147|0.0468|0.9328|0.9790|0.9553|0.9563|
|B7+UNet|0.9153|0.0461|0.9332|0.9792|0.9556|0.9566|

### Building Segmentation

### Road Segmentation