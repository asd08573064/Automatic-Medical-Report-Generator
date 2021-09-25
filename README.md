# Automatic-Medical-Report-Generator

## Model

we use a CNN model, the encoder, to learn the visual features from the chest X-ray images, then these learned features will be representative of the image. Next, we pass the representation to the transformer to generate a sequence of data, which is the final prediction of the caption. See the link to understand Transformer https://www.tensorflow.org/text/tutorials/transformer



## Dataset

The Indiana University Chest X-ray Collection (IU X-Ray) (Demner-Fushman et al., 2015) is a set of chest x-ray images paired with their corresponding diagnostic reports. The dataset contains 7470 reports paired with their corresponding X- ray images. 
### NIH

https://openi.nlm.nih.gov/detailedresult?img=CXR111_IM-0076-1001&req=4

### Kaggle

https://www.kaggle.com/raddar/chest-xrays-indiana-university/activity


##Result



<img width="140" alt="截圖 2021-09-25 下午9 56 44" src="https://user-images.githubusercontent.com/43490777/134774027-0546323a-0690-4e3d-b669-bec4c222fba2.png">
*Prediction: he cardiomediastinal silhouette is within normal limits. no fo- cal airspace consolidation. no pneumothorax or large pleural effusion. visualized osseous structures are unremarkable. no acute abnormality.

*Ground: no acute osseous abnormality. soft tissue structures are within normal limits. stable normal cardio mediastinal silhouettes and hilar structures. the lungs are normally inflated without evidence of focal airspace disease, pleural effusion, or pneumothorax.

<img width="145" alt="截圖 2021-09-25 下午9 57 51" src="https://user-images.githubusercontent.com/43490777/134774067-04aa4818-6638-4031-9789-22829cdab472.png">
*Prediction: heart size and pulmonary vascularity appear within normal limits. no pneumothorax or pleural effusion. There is a mild right hilarious cal- cification which could represent scarring. no focal airspace consolidation is seen. hyperexpanded lungs.
*Ground: heart size and pulmonary vascularity appear within normal lim- its. The lungs are free of focal airspace disease. no pleural effusion or pneumothorax is seen. vascular calcification is noted. no evidence of active disease.


<img width="138" alt="截圖 2021-09-25 下午9 58 00" src="https://user-images.githubusercontent.com/43490777/134774078-7b887e0e-3b74-46ad-9480-b2d7c3ba51c0.png">
*Prediction: the trachea is midline. the cardiomediastinal silhouette ap- pears normal. The lungs are clear, without evidence of focal consolidation or effusion. There is no pneumothorax. The visualized osseous structures reveal no acute abnor- malities.no acute cardiopulmonary abnormalities.
*Ground: normal heart size. normal pulmonary vasculature. normal medi- astinal contours. lung parenchyma is clear. no airspace disease. no pulmonary edema.
