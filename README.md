# Classifying Breast Cancer Tumor types
By Himasri Mora Reddy

Breast cancer is the most common cancer in women. Early diagnosis of Breast cancer that can improve the prognosis and chance of survival significantly and a hospital wants to create an automated way to detect the cancer type. So the goal is to classify whether the breast cancer tumor is benign or malignant using the data from the State of Wisconsin. A Logistic Regression model was chosen to be the optimal model and achieved a 97% true positive rate for predicting Malignant tumor type.

<p align="center" width="100%">
<img src="https://github.com/hmorareddy/AI_Capstone/blob/main/image.png" alt="breast cancer logo" height="480" width="640"/>
</p>

## Business Understanding & Problem

Breast cancer is the most common cancer in women, accounting for 1 in 4 cancers diagnosed in the U.S. and causing over 40,000 deaths each year, and it is the second leading cause of cancer death among women, after lung cancer. Breast Cancer occurs as a result of abnormal growth of cells in the breast tissue, commonly referred to as a Tumor. A tumor does not mean cancer - tumors can be benign (not cancerous), pre-malignant (pre-cancerous), or malignant (cancerous).

Early detection of breast cancer is key and can help improve the chances of survival. A research shows that the doctors are only able to detect 70–80% accurately which might cause a serious threat to the undiagnosed patients suffering from breast cancer. A hospital wants to create an automated sytem to detect if the cancer diagnosed is malign or benignant, using information such as their mean radius, mean compactness, worst area etc.

Classification model built will be used by the hospital to determine if the patient has malignant cancer or not and this could help in early diagnosis of Breast cancer that can improve the prognosis and chance of survival significantly, as it can promote timely clinical treatment to patients.Further accurate classification of benign tumors can also prevent patients undergoing unnecessary treatments.

## Data Understanding

The dataset consists of several human cell sample records, each of which contains the values of a set of characteristics of the nucleus. Here is a **[link](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)** to the dataset. It is available as machine learning repository maintained by the University of California, Irvine.

<strong>Features computed from each cell nucleus:</strong>

- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter
- area
- smoothness (local variation in radius lengths)
- compactness (perimeter^2 / area - 1.0)
- concavity (severity of concave portions of the contour)
- concave points (number of concave portions of the contour)
- symmetry
- fractal dimension ("coastline approximation" - 1)
<br>

<strong>Expected outcome </strong>

Given breast cancer results from breast fine-needle aspiration (FNA) test (is a quick and simple procedure to perform, which removes some fluid or cells from a breast lesion or cyst (a lump, sore, or swelling) with a fine needle similar to a blood sample needle). The features have been computed from digitized images of the cell nuclei, which can be used to build a model to predict whether a tumor is benign or malignant.
* 1 = Malignant (Cancerous) - Present
* 0 = Benign (Not Cancerous) -Absent
