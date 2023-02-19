# Land-cover classification using MA-Net model
This project is a land-cover classification task using the MA-Net model. The goal is to classify satellite imagery into various land-cover classes, such as forest, water, agriculture, etc.

# Dependencies
* pytorch-lightning
* segmentation-models-pytorch
* albumentations
* torchinfo
* pandas
* matplotlib

# How to Run
* Download the .ipynb file 
* Download the DeepGlob dataset
* Keep the dataset in Google Drive
* Open the .ipynb file in Google Colab
* Mount the Google drive 
* update the dataset drectory in the code
* run in Google Colab

# Dataset
We have used the land cover dataset [1] that contains a collection of 1949 satellite images. This dataset is used to detect areas of urban, agriculture, rangeland, forest, water, barren, and unknown. There is a mask for each of the images which indicates the position of the categories of land cover.

<img width="424" alt="Screen Shot 2023-02-19 at 12 29 44 AM" src="https://user-images.githubusercontent.com/24860187/219926779-1ce6c20f-6e94-445e-ab73-3899c385bebb.png"> 
<img width="395" alt="Screen Shot 2023-02-19 at 12 30 03 AM" src="https://user-images.githubusercontent.com/24860187/219926814-6f5061a4-b09b-408c-a153-43928c8efd8c.png">

# MA-Net Model
The MA-Net model is a deep learning architecture that has been shown to achieve state-of-the-art results in land-cover classification tasks. The model consists of multiple attention modules that selectively attend to different regions of the input image.
<img width="432" alt="Screen Shot 2023-02-19 at 12 26 44 AM" src="https://user-images.githubusercontent.com/24860187/219926038-596f7fa1-4230-496b-8c16-ba5459297fce.png">

# Results
Our experiment shows that the MAnet model can provide outstanding performance in terms of accuracy, IoU, precision, recall and F1 score on land cover dataset which are better than Unet++

<img width="446" alt="Screen Shot 2023-02-19 at 12 13 46 AM" src="https://user-images.githubusercontent.com/24860187/219923912-4a262f13-8ead-4d2d-9200-9ae384be0ab4.png">

# Reference
[1] Demir, Ilke, et al. "Deepglobe 2018: A challenge to parse the earth through satellite images."   Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. 2018.

[2] T. Fan, G. Wang, Y. Li and H. Wang, "MA-Net: A Multi-Scale Attention Network for Liver and Tumor Segmentation," in IEEE Access, vol. 8, pp. 179656-179665, 2020, doi: 10.1109/ACCESS.2020.3025372.

[3] Wu, Yuxin, and Kaiming He. "Group normalization." Proceedings of the European conference on computer vision (ECCV). 2018.

[4] LU HTOO KYAW ‘Landcover ClassificationUNet++’https://www.kaggle.com/code/luhtookyaw/landcover-classification-unet

[5] Rost, ‘DeepGlobe land cover classification’https://www.kaggle.com/code/rostekus/deepglobe-land-coverclassification/notebook

[6] Yao Li and Luo Chen, deepglobe land cover classification with deeplabv3plus ’https://github.com/GeneralLi95/deepglobe_land_cover_classification_with_deeplabv3plus
