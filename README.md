#  Image Classification of Grape Leaf Diseases Using VGG16-based Deep Learning Model

Datasets used in this project

1. Plant leaf grapes only Dataset (used in the assignment, subset of Plant Village dataset):

https://drive.google.com/drive/folders/1usFmL0ox7Sev7IB7QCm_qFV6HHFtci-N?usp=drive_link


2. Plant Village Dataset:

 https://data.mendeley.com/datasets/tywbtsjrjv/1


# Problem Statement
In the landscape of precision agriculture, the problem lies in the development of a robust computer vision system that could seamlessly and effectively classify images or objects in the agricultural area. The traditional state of computer vision in the detection of crop diseases and pests requires more improvement and innovations. Traditional computer vision in crop disease and pest detection usually incorporates conventional image processing algorithms and manual feature engineering, together with classifiers (Sinha & Shekhawat, 2020). This approach usually involves scheme designs that are built on the specific properties of the crop. In real situations, various factors such as minor differences in the backgrounds, lesions and noises in the crop images could potentially cause inaccuracies in the method (Liu et. al., 2017; Sinha & Shekhawat, 2020). Fortunately, the advancement of deep learning has provided a promising solution. However, even with deep learning as the approach, there are also hurdles in the application. The development of deep learning models from scratch presents challenges such as data scarcity and limited computational resources. The scarcity of labelled datasets for the agricultural industry further increases the difficulty level as data scarcity will affect the generalisation of models. Thus, alternative approaches such as transfer learning that employs pre-trained models can be explored in this domain to develop deep learning-based image classifiers to detect grape leaf diseases. This is because pre-trained models are usually trained on large-scale datasets and reusing the knowledge of pre-trained models could reduce the requirements.

# Experimental Design
##Dataset description
A publicly available PlantVillage dataset is obtained from the Mendeley database (J & Gopal, 2019). The dataset consists of approximately 61,486 RGB images and it is alleged to be the largest crop database in the world. These images comprised healthy and unhealthy crop images from 39 categories of crop specifies and diseases. In this project, only grape leaf images will be used for the experiment of this project. There will be 4 classes in the grape leaf dataset.
# Methodology
This experiment will develop convolutional neural network (CNN) models for the image classification of grape leaf diseases using the VGG16 architecture. This project will adopt transfer learning and other configurations to enhance the model performance to achieve the objectives.
In this project, VGG16 pre-trained model will be chosen because of its effectiveness in computer vision-related tasks such as image classification. Using the pre-trained weights from the VGG16 pre-trained model, the features extracted from the large-scale dataset can improve the representation of the proposed model and expedite the training process in this project (Simonyan & Zisserman, 2014).

After the data collection, preprocessing and augmentation, the initial step will involve the training of two models using different configurations and architectures. The first model will be a VGG16-based model with all the convolutional layers frozen. The pre-trained weights of the VGG16 will be retained in this model. Next, for the second model of the VGG16-based model, only the layers in the block 5 convolutional block will be trainable. After both the models are trained using the Plant Village Grape dataset, the models will be evaluated using metrics such as accuracy and loss. The performance of the models will be compared, and the well-performed model will be chosen for further optimization and fine-tuning. The chosen model will undergo a fine-tuning process such as unfreezing additional layers and changing the learning rate and dropout rate. Ultimately, there will be a total of 5 models in this project, 2 are the initial proposed models and the remaining 3 models will be the fine-tuned models.
