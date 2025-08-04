# Model Card

## Model Description

- **Input:**

  The model takes <b>32 data</b> as input :

  - <b>Demographic details</b> : Age, Gender, Ethnicity and EducationLevel.
  - <b>Lifestyle factors</b>: BMI, Smoking, Alcohol Consumption, Physical Activity, Diet Quality and Sleep Quality.
  - <b>Medical History</b> : Family History with Parkinson's Disease, Traumatic Brain Injury, Hypertension, Diabetes, Depression and Stroke.
  - <b>Clinical Measurements</b> : SystolicBP, DiastolicBP, Total Cholesterol, LDL Cholesterol Level, HDL Cholesterol level and Triglycerides level.
  - <b>Functional Assessments</b> : Unified Parkinson's Disease Rating Scale score (UPDRS), Montreal Cognitive Assessment score (MoCA) and Score from a functional assessment.
  - <b>Symptoms</b> : Presence of tremor, presence of rigidity, presence of bradykinesia, presence of postural instability, presence of speech problems, presence of sleep disorders and presence of constipation 


- **Output:** 
  - <b>Diagnosis</b>: The model outputs the Diagnosis status for Parkinson's Disease (0 for No, 1 for Yes).

- **Model Architecture:** 
  - The model is based on <b>XGBoost</b> (eXtreme Gradient Boosting) which got the best results both for <b>accuracy</b> and <b>recall</b> among 6 pre-chosen models.
  - Hyperparameters of the model have been optimized with <b>Bayesian Optimization</b>, which gave better results than other methods.
 
<br>

## Performance
  - The model got an accuracy of 94,3% and a recall of 96,6%.
  - The performances were measured on test set that was built by the train_test_split method of the sklearn library.
  - The test set consisted in 421 samples from the initial dataset (2105 samples).

<br>

## Limitations
- <b>Techical Limitations</b> 
  - Six models were initailly tested. We could have tested a few more that could possibly got even better results. 
  - Hyperparameters tuning was only performed on the model that got the best results on the initial run. We could possibly got better results with hyperparameter tuning of other models. 
  - Some binary data were highly unbalanced (specially in the medical history data). This can lead to biases in modeling.
- <b>Medical Limitations</b> 
  - The model measures the presence or absence of the disease. It does not indicate its intensity. However, this data is key in the management of the disease. Each patient requires a very distinct approach.
  - The dataset only includes 2105 samples, which remains rather low for effective generalization.

<br>

## Trade-offs
  - During the tuning phase, we prioritized the recall score to minimize False Negatives. We did not measure the impact on the False Positive detection rate. However, it is common for optimization of one to be at the expense of the other.
  - The model is operational because the measurement of a number of criteria is binary. In the context of more nuanced measures (e.g., numerical scale) for these data, the model would have to be reconstructed.
