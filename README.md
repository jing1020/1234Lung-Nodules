# 1234Lung-Nodules

Classification of Malignancy of Lung Nodules

 1. Project introduction
 
	This project aims to develop a statistical model for lung disease detection and classify the Malignancy of lung Nodules. The data I was using is from the Lung Image Database Consortium image collection (LIDC-IDRI) and Tianchi Data Lab on Alibaba Cloud. The project used techniques for image processing and classification algorithms in machine learning and deep learning. 

2. Preprocessing data

	Data preprocessing included reading images in DICOM data type, decoding XML file to get radiologist annotations.

3. Lung Nodules Segmentation and Feature Extraction

	3.1 Lung Nodules Segmentation: Applied 3-dimensional CNN model to locate regions of interest (roi) within the lung based on the location information given in LIDC dataset. The input of this process is computed tomography (CT) images for each patient. The output of this process is roi - a cube (	L = 56mm) containing lung nodule in it.
	3.2  Feature Extraction: Extracted lung nodule features based on the contour information given by LIDC dataset including nodule location, hu value, longest radius, cross sectional area, etc.

4. Classification of Malignancy of Lung Nodules

	Used several algorithms to classify the malignancy of nodules based on extracted features including KNN,SVM and CNN. The    training and testing dataset is from LIDC and Tianchi Data. For testing dataset, we had a doctor team to mark the contour of lung nodule and diagnosed the  malignancy of nodules in person. The accuracy of prediction reached 85%.
