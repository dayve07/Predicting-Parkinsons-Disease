# Model Card

## Model Description

- **Input:** The model takes 33 data as input :

  - Demographic details : Age, Gender, Ethnicity and EducationLevel.

  - Lifestyle factors: BMI, Smoking, Alcohol Consumption, Physical Activity, Diet Quality and Sleep Quality.
  - Medical History : Family History with Parkinson's Disease, Traumatic Brain Injury, Hypertension, Diabetes,  Depression, Stroke.
  - Clinical Measurements : SystolicBP, DiastolicBP, Total Cholesterol, LDL Cholesterol Level, HDL Cholesterol level and Triglycerides level.
  - Functional Assessments : Unified Parkinson's Disease Rating Scale score (UPDRS), Montreal Cognitive Assessment score (MoCA), Score from a functional assessment.
  - Symptoms : Presence of tremor, presence of rigidity, presence of bradykinesia, presence of postural instability, presence of speech problems, presence of sleep disorders and presence of constipation 


- **Output:** 
  - Diagnosis: The model outputs the Diagnosis status for Parkinson's Disease (0 for No, 1 for Yes).

- **Model Architecture:** 
  - The model is based on XGBoost (eXtreme Gradient Boosting) which got the best results among 6 pre-chosen models.
  - Hyperparameters of the model have been optimized with Bayesian Optimization, which gave better results than other methods.
 
<br>

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
