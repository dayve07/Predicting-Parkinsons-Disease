# Datasheet


## Motivation

- <b>For what purpose was the dataset created?</b>

  This dataset was created for researchers and data scientists aiming to explore factors contributing to Parkinson's Disease, develop predictive models, and conduct statistical analyses.
    
 - <b>Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?</b>
 
   - This dataset was shared by Rabie El Kharou on kaggle.com. We don't have any specifications on who specifically created the initial dataset but the dataset has likely been created for educational purposes.
   - I don't have any reliable information about Mr. Rabie El Kharou's profile. However, Mr. Rabie El Kharou has a recognized account on kaggle.com and appears in several search results as an AI and Machine Learning Student. However, I cannot certify that this is the same person.

<br>
 
## Composition

- <b>What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)</b>

  - The instances represent medical information of 2105 patients. The dataset includes demographic details, lifestyle factors, medical history, clinical measurements, cognitive and functional assessments, symptoms, and a  diagnosis indicator, indicating if the patient has the Parkinson's Disease or not.
  - Data is numerical for lifestyle factors, clinical measurements, functionnal assessments. Data is binary for symptoms and medical history. DAta is categorial for some demographic details (ethnicity and Eductaion Level).

- <b>How many instances of each type are there?</b>

  There are 2105 instances.

- <b>Is there any missing data?</b>

  There's no missing data.

- <b>Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?</b>

  The dataset contains highly confidential data as it comprises health information. Nevertheless, the Patient's ID and the Doctor in Charge have been previously anonymized. 

<br>

## Collection process
- <b>How was the data acquired?</b>

  Unknown to the author of the datasheet.
  We know that this dataset is synthetic and was generated for educational purposes but we do not know how the initial data was acquired.
  
- <b>If the data is a sample of a larger subset, what was the sampling strategy?</b>

  Patients are all over 50 years old but we are not able to conclude that this was part of a sampling strategy.
  
- <b>Over what time frame was the data collected?</b>

  Unknown to the author of the datasheet.

<br>

## Preprocessing/cleaning/labelling
- <b>Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.</b>

  Unknown to the author of the datasheet.

- <b>Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?</b>

  <i>n/a</i>

 
<br>
 
## Uses

- <b>What other tasks could the dataset be used for?</b>

  This dataset can be used as a reference for developing datasets for the detection of other diseases. The factors that influence the onset are essentially the same as those in this dataset.

- <b>Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms?</b>

  - This dataset specifies the patient's ethnicity. The use of this data requires special care. Generalization of results and studies must be conducted with careful caution. 
  - Much data is binary, which doesn't allow for nuance, especially for symptom-related data. This can introduce significant bias into analysis and conclusions.

- <b>Are there tasks for which the dataset should not be used? If so, please provide a description.</b>

Due to its educational nature, this dataset should not be used in a professional or medical setting. However, it can be used as a source of inspiration to develop real and usable datasets.

<br>

## Distribution

- <b>How has the dataset already been distributed? </b>

  It is distributed by Kaggle : https://www.kaggle.com/datasets/rabieelkharoua/parkinsons-disease-dataset-analysis.
  There might also be other places where the dataset is available.
  The author of the datasheet do now know when it first became publicly available, but the datacard on kaggle was last edited in 2024.  

- <b>Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)? </b>

  It is made available under the CC BY 4.0 license, allowing anyone to use the dataset in any form as long as proper citation is given to the author. 

<br>

## Maintenance

- <b>Who maintains the dataset?</b>

Unknown to the author of the datasheet.

