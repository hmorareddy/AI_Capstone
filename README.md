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

![image](https://user-images.githubusercontent.com/110204917/216629877-f3a9672e-f0ff-47ad-82b4-0ee4554aa211.png)

* There are 357 Benign and 212 cancer tumor categories

Removed unnecessary columns and there are no missing values in the data.

![image](https://user-images.githubusercontent.com/110204917/216631007-a66d04de-4935-4c44-b752-e72ce2b3d45b.png)

* We can clearly see that several columns are very highly correlated, causing multicollinearity among independent variables. After analysing the above plot, columns with a threashold value of above 0.85 have been removed from the dataset 

## Modeling and Evaluation

Two classification models were built - Logistic Regression and Decision Tree. They were optimized with GridSearchCV.

The metrics used to evaluate the model performance is Recall. Recall is crucial in this scenario to correctly detect the Malignant(cancerous) tumor types so that the hospital could provide an early treatment to the patients. 

**Models Performance **
| Model |  Recall |
|-------|----------|
| Logistic Regression | 97% |
| Decision Tree| 94% |

Logistic regression model achieved 97% true positive rate and Random forest got a recall(true positive rate) score of 94%

## Conclusion

- Logistic regression had the highest true positive rate of 97% when compared to the Decision Tree model. Hence, Logistic Regression is chosen as the best model to predict the tumor categories.One of the limitations is that the training data used is small and one of the next steps would be to train a model on neural network on a larger sample of data.

## Repository

**An explanation of the repository organization**
- Data : folder for Breast Cancer tumor dataset used for this project
- index.ipynb : jupyter notebook for EDA, data cleaning, modeling and evaluation
- Presentation.pdf : final presentation slides

**Links to the final notebook and presentation**
- [index.ipynb](.//index.ipynb)

**Reproduction instructions**
- Download the [dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) available on Kaggle.
- Download [index.ipynb](.//index.ipynb) and open it on Google Colab or Jupyter Notebook to run 
