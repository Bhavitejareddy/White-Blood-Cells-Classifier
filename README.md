# White Blood Cell Classification 


Live Hosted Web Link: [🚀 Visit Live Website](https://wbc.onrender.com/)<br>
Video Demo: [📺 Watch the Video Demo](https://www.youtube.com/watch?v=1NqH9XWJdNA)

## Project Members:
* Jinka Chandra Kiran
* Kokkula Lokesh
* Tatigunta Bhavi Teja Reddy


## Publication:
This project was published in EAI Endorsed Transactions on Pervasive Health and Technology. [Link](https://www.researchgate.net/publication/377426875_White_Blood_Cells_Classification_using_CNN
)

![image](https://github.com/user-attachments/assets/40d15bfa-95ee-4ed1-b028-0bba37375d35)

## Overview

Leukemia is a type of blood cancer that is caused by the abnormal production of white blood cells (WBC). Proper diagnosis and treatment are critical, as leukemia is caused by different types of WBCs, and misdiagnosis can lead to severe complications for the patient. This project focuses on identifying the type of WBC causing leukemia using image classification techniques, leveraging deep learning models.

We utilize Convolutional Neural Networks (CNN), Artificial Neural Networks (ANN), and ensemble techniques to classify WBCs from images.

This repository contains code and resources for a 4-class classification task of white blood cells. The objective is to classify white blood cell images into four different classes based on their morphology.

![image](https://github.com/user-attachments/assets/02e0f6ef-1610-4117-9e47-86c343f77106)

## Problem Statement

Leukemia, a form of bone marrow disorder, is caused by the abnormal production of white blood cells. Accumulation of these cells restrains the production of healthy blood cells, potentially leading to anemia, infections, internal bleeding, and tumor formation. With different types of leukemia stemming from various kinds of WBCs, it is essential to accurately identify the type of WBC responsible to determine the right course of treatment.

## Dataset

The dataset used for this project was collected from the Kaggle platform and contains 1200 images of white blood cells across 4 classes. The images are labeled and annotated, providing a comprehensive representation of the morphological changes in WBCs. Noise in the images was reduced using outlier techniques, improving classification accuracy.

1. Neutrophils
2. Lymphocytes
3. Monocytes
4. Eosinophils

## Proposed System

Each image from the dataset includes a WBC cell that is highlighted in blue, as well as a little amount of blue-colored noise, as shown in the figure 4. We employed a method known as outlier technique to lessen this noise. A data point in a dataset that is significantly far away from the other values in the same dataset is referred to as an outlier. Outliers might be the consequence of measurement errors, data entry mistakes, or real observations that are just infrequent or unexpected. Outliers can have a substantial impact on a dataset's analysis and lead to inaccurate conclusions if they are not handled properly. Now these far away blue colored noise has to be reduced in the dataset. So here we basically get the pixels of the whole image in both x and y axes, and collects all blue color pixels. Now outliers’ technique will take the coordinates of both x and y axes values and checks the closely packed pixels and far away pixels, then it removes the pixels which are far away from the closely packed ones.

![Alt text](image.png)

After eliminating the noise in the data, we cropped the image so that only the blue-highlighted portion was transferred to the data, potentially improving accuracy. By determining the intersection locations of the lines created by the maximum and minimum values of the x-axis and y-axis of pixels of the highlighted blue region, this cropping is performed. To make the generated final image easier to read, we extended the lines' pixel length. The final image is shown in figure 5 below

![Alt text](image-1.png)


 ## Work Flow

1.	Data gathering: Gathering a sizable number of digital photographs of white blood cells from diverse platforms, such flow cytometry or microscopy.
2.	 Data preparation: Enhancing the characteristics for better classification by preprocessing the pictures to eliminate any noise, normalize the color and contrast, and remove any artefacts.
3.	Feature extraction: To identify different types of white blood cells and their properties, features are extracted from the pictures using deep learning techniques like convolutional neural networks (CNNs).
4.	Model training: Improving the classification accuracy of white blood cells by teaching a machine learning or deep learning model, such as a CNN, the retrieved characteristics.
5.	Model evaluation involves assessing the trained model's performance on a different test dataset and refining the model's parameters for increased precision and productivity.


![Alt text](image-2.png)

 ## Results

Using the CNN model, we achieved an accuracy of 93% on the BCCD dataset, which contains 12,000 images of WBCs. Additional models such as ANN and ensemble methods were also used, but CNN outperformed them with the highest accuracy.
Algorithm	  | Accuracy
------------- | -------------
CNN	  | 93%
SVM  | 87%
KNN	|82%
ANN	|67%

## Future Work

* **Enhance Feature Extraction**: Explore additional methods such as transfer learning and attention-based models.
* **Expand Dataset: Incorporate** more diverse datasets to improve model generalizability.
* **Real-World Application**: Implement user studies to evaluate the model's usability in clinical environments.
## For More Details 
[Download the PDF here](https://docs.google.com/document/d/1krJ3hxspWHM_Qm4x0UJd70a3FybMealv/edit?usp=sharing&ouid=109596835077990572925&rtpof=true&sd=true)



