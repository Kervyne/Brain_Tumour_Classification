# Brain_Tumour_Classification

## Brain Tumour Classification with Support Vector Machine (SVC)

### Background and Problem Statement

In Singapore, there are over 500 adults and 40 young childrens going for surgical treatments of their brain tumours annually, just in public hospital alone.
<br><br>
Brain tumors represent a significant health challenge worldwide, with a wide range of tumor types, varied clinical presentations, and diverse treatment options. While advancements in imaging techniques such as MRI have improved the detection and characterization of brain tumors, challenges persist in accurately diagnosing, classifying, and effectively treating these tumors. Misdiagnosis, inadequate treatment strategies, and the lack of effective targeted therapies contribute to the morbidity and mortality associated with brain tumors. 
<br><br>
Additionally, the heterogeneity of brain tumors presents a significant obstacle in developing personalized treatment approaches. Furthermore, it may also cause significant symptoms, affecting the quality of life. Therefore, there is an urgent need for further research to enhance our understanding of brain tumor biology, improve diagnostic accuracy, refine treatment strategies, and develop targeted therapies to improve patient outcomes and quality of life. As such, early diagnosis and identification of brain tumour is essential to provide timely treatment.
 <br><br>
 
The aim of this project is to develop an image classification model using computer vision techniques to accurately classify common brain tumours, specifically pituitary tumour, meningioma tumour and glioma tumour, or no tumour. The model should aid and complement in obtaining a preliminary diagnosis of various brain conditions.

**Source** <br>
[Brain Tumour Society Singapore](https://www.braintumoursociety.org.sg/basic-facts-about-brain-tumours/) <br>
[Primary Brain Tumors in Adults: Diagnosis and Treatment](https://www.aafp.org/pubs/afp/issues/2016/0201/p211.html)
<br>
### Objectives

- To develop an image classification model with Support Vector Machine (SVC) using training MRI images and accurately categorize 4 different classification (pituitary tumour, meningioma tumour and glioma tumour, or no tumour)<br>
- To apply the trained model on new, unseen MRI images to accurately categorize and predict the brain tumour or no tumour
<br><br>
### Data

##### Data Source
[Brain Tumour Classification (MRI) from Kaggle](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)

**Training Folder** <br> glioma_tumor: 826 images <br> meningioma_tumor: 822 images <br> no_tumor 395 images <br> pituitary_tumor: 827 images <br><br>
**Testing Folder** <br> glioma_tumor: 100 images <br> meningioma_tumor: 115 images <br> no_tumor: 105 images <br> pituitary_tumor: 74 images

### Results
| Metric                         | Training Score | Testing Score |
|--------------------------------|----------------|---------------|
| Accuracy                       | 0.94           | 0.83          |
| Precision (weighted)           | 0.94           | 0.83          |
| Recall (weighted)              | 0.94           | 0.83          |
| F1 Score (weighted)            | 0.94           | 0.83          |

- Principal Component Analysis was not implemented as the data is highly non-linear

### Conclusion

The model is fairly accurate to serve as a reliable tool for preliminary diagnosing brain tumours<br>
- As seen from the results, it has achieved ~83.0% accuracy.
- Not only that, it also achieved ~83.0% for all other parameters, providing a good balance for all metrics.<br>

In conclusion, I have successfully trained and developed an image classification model with Support Vector Machine modeling in this project to predict brain tumors fairly accurately. This comprehensive solution provides healthcare providers with the means to obtain reliable preliminary findings. This should complement the knowledge of medical professionals to obtain an accurate diagnosis for the patient.

## Recommendations 

1. Incorporation with healthcare institution and collaboration with radiologists<br>
- This is not meant to replace radiologist fully in providing diagnosis for the patient, but rather aids and complements with the knowledge that they have, making it a more seamless and faster process of providing a diagnosis for the patients <br>
- A by-product of such modelling can also be considered to be integrated into a telemedicine features and digitalisation of medical images, providing patients the convenience of obtaining their images without the need of leaving their houses<br><br>
2. Continuing modelling improvement and alternative models with expansion of dataset<br>
- More data, particularly from Singapore, can be collected to expand the dataset to improve the model's reproducibility and capability in the local context<br>
- Alternative modelling such as deep learning algorithms can be considered especially with a larger dataset to better handle the increased complexity in the future
