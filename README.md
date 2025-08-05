# **Predicting Parkinson's disease using Machine Learning**

# **💡Context**

 * **Parkinson’s Disease** (PD) is a **degenerative neurological disorder** that irremediably decreases mental faculties and movement.

 * Due to the aging of the population, **the disease affects an ever-increasing proportion of the population**.

 * As with many diseases, **early detection is crucial for anticipating future treatments** and helping patients make necessary adjustments to their daily lives.
 
 * **Traditional detection through medical imaging is still expensive, invasive and time-consuming**. Detecting the disease using other techniques is a key issue in managing the disease.

<br>

# **🎯Project Goals**

* This project is aimed to **predict if an adult has the Parkinson Disease (PD) or not** by using AI and Machine Learning techniques. These techniques, that have emerged these last years offers an credible alternative to tradionnal detection.

* Based on **35 factual indicators** mainly regarding some **clinical measurements, medical history and cognitive assessments** of the patient, we will seek a way to predict the presence or absence of Parkinson's disease.
  
* Our prediction must be as accurate as possible; we also set the objective of minimizing the number of False Negatives in our results (detection of a healthy patient when he has the disease).

<br>  

# **🔬 Dataset**
* The study is based on a **dataset made available on the [kaggle.com](https://www.kaggle.com/datasets/rabieelkharoua/parkinsons-disease-dataset-analysis) platform**.

* The dataset is under **[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) Licence** since 2024.

* Author : **Rabie El Kharoua. (2024)**. 🏥Parkinson's Disease Dataset Analysis🧠 [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/8668551

<br> 

# **⚛Model** 
* The model is based on XGBoost (eXtreme Gradient Boosting) which got the best results both for accuracy and recall among 6 pre-chosen models.

* XGBoost, is a model known for its speed and ability to process a large number of parameters. It is technically based on 

<br> 

# ⚖ **Hyperparameter Optimisation**
* Here are the best hyperparameters found by **Bayesian optimization** (hyperopt library) :
  
   ➡ **'colsample_bytree': 0.805** / prevents overfitting, by selecting 80% of the features for each sub-tree
  
   ➡ **'learning_rate': 0.078** / low value that should lead to better generalization

   ➡ **'max_depth': 3.0** / prevents overfiiting, by constructing ratger small sub-trees

   ➡ **'n_estimators': 267.0** / moderate number of subtrees, that helps balance between generalization and overfitting

   ➡ **'subsample': 0.750** / prevents overfitting, by selecting 75% of the samples for each subtree. This adds another layer of randomness. 

* These hyperparameters have all been chosen **to prevent overfitting** and **maximize generalization**.

<br> 

# ✅ **Results**

*   **We now have a fully operational model at our disposal**. We have built a machine learning model to predict Parkinson's disease. The results regarding the various metrics are very satisfactory. **The accuracy is almost 95.0%**, but we have also managed to minimize the number of False Negatives (**recall is 96.9%**), which is always a major objective in the case of detecting disabling diseases.

*   **Clinical assessment scores** (UPDRS, MoCA, FunctionalAssessment) and **key symptoms** (Tremor, Rigidity, Bradykinesia, PosturalInstability) are the most influential features in predicting Parkinson's disease.

*   **Such a model can help doctors factualize a diagnosis**. It obviously does not replace a consultation and examinations with qualified doctors or specialists; but it can be a valuable aid.

<br> 

#  ⏰**Further investigations:**

*   **Many features in our dataset were binary**, so they may lack nuance depending on the affected patient. Greater symptom refinement may help improve the model and its future use.
*   **Regarding speech problems, numerous datasets are available** to detect the presence or at least a suspicion of Parkinson's disease in voice variations. Combining our dataset with a dataset of this type would allow us to seriously refine the model.
*   While detection is of course key, **monitoring the progression of the disease is just as important**. Our model could potentially serve as a basis for this other type of modeling.

<br> 
You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

