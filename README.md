# SHAP_Values_for_Suicide_Study
### SHAP Value Methods was applied to check the associations between suicide rates and rurality, altitude, climate factors, and social economic factors from 2010 to 2020. Suicide rates are divided to 3 groups: suicide by all means, suicides by firearms, suicides by non-firearms. SHAP values are investigated in each single year and multiple 5-year periods such as 2010 to 2014, 2011 to 2015 ans so on.

### Climate Factors includes mean temperature, visibility, precipitation and so on. The code to collect climate data can be found here:  [Climate Factors](https://github.com/Wenhuan2516/Climate-Data-Scraping)
### Social economic factors includes poverty, unemployment, disabled, and so on. The code to collect social economic data from Census API can be found here: [Social Economic Factors](https://github.com/Wenhuan2516/Census-API-data-collection)
### Since only about 1000 counties have the suicide death records from CDC, I imputed the suicide rates by assigning the average suicide rates from the abjecent counties. The code to impute suicide rates can be found here: [Suicide Rate Imputation](https://github.com/Wenhuan2516/SuicideRatesDataImputation)
### Here I am using SHAP Values in year 2016 as an example to show you how I built the model and get the results.
### More results can be found here: 
#### 1. [Comparing SHAP Values from 3 Suicide Groups: Firearm, Non-firearm, Overall - Part 1](https://docs.google.com/document/d/1a5n9hVakSRV7vyuA8BnJeFJOQsP3kQMCQUoidGKAG7Y/edithttps://docs.google.com/spreadsheets/d/1GFkTjwwtsrosPP1TxGRUbvjTnRfd93Ue7KA-q9mi0_0/edit?usp=sharing)
#### 2. [Comparing SHAP Values from 3 Suicide Groups: Firearm, Non-firearm, Overall - Part 2](https://docs.google.com/spreadsheets/d/1KJ320LvVQbWP12vRKhsnmRINnWyhSWS0I8k6j6rvGTo/edit?usp=sharing)
#### 3. [Random Forest Importance Result](https://docs.google.com/spreadsheets/d/1czFfLy2hyC_0OMusSJ3q0do9tUBPt-lNBH9LBqu_M00/edit?usp=sharing)
#### 4. [Suicide Rate Analysis](https://docs.google.com/spreadsheets/d/1AwO5qR4En9ASxsBAuejjg8Yq8GP-LyQqsUhbX7E2VKg/edit?usp=sharing)

### The report for this project can be found here: [Developing Interpretable Method to Understand Feature Importance and Interactions for for Suicide Risk Management](https://docs.google.com/document/d/1a5n9hVakSRV7vyuA8BnJeFJOQsP3kQMCQUoidGKAG7Y/edit?usp=sharing)
### The poster looks like this:
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/poster1.png" alt="County Adjacent File" title="Poster1">
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/poster2.png" alt="County Adjacent File" title="Poster2">

### Random forest method was used to check the feature importance before SHAP Value method was applied.

#### Random Forest Feature Importance for Climate Factors 
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/random2.png" alt="SHAP result" title="shap1">

#### Random Forest Feature Importance for Social Economic Factors 
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/random1.png" alt="SHAP result" title="shap1">

#### Random Forest Feature Importance for All factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/random3.png" alt="SHAP result" title="shap1">

### SHAP Values for Overall Suicide rates(Suicide death caused by firearms and Non-firearms)
#### Plot bar graph to rank SHAP values for climate factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-1.png" alt="SHAP result" title="shap1">

#### Beewarm graoh to rank SHAP values for climate factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-2.png" alt="SHAP result" title="shap1">

#### Interaction between elevation/altitude(y-axis) and rurality(x-axis)
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-4.png" alt="SHAP result" title="shap1">

#### Interaction between elevation/altitude(x-axis) and rurality(y-axis)
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-5.png" alt="SHAP result" title="shap1">

#### SHAP Value of social economic factors for one county as an example
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-6.png" alt="SHAP result" title="shap1">

#### Plot bar graph to rank SHAP values for social economic factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-7.png" alt="SHAP result" title="shap1">

#### Beewarm graoh to rank SHAP values for social economic factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-overall-8.png" alt="SHAP result" title="shap1">

### SHAP Values for Firearm Suicide rates(Suicide rates by Firearm)
#### Plot bar graph to rank SHAP values for climate factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-1.png" alt="SHAP result" title="shap1">

#### Beewarm graoh to rank SHAP values for climate factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-2.png" alt="SHAP result" title="shap1">

#### Interaction between elevation/altitude(y-axis) and rurality(x-axis)
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-3.png" alt="SHAP result" title="shap1">

#### Interaction between elevation/altitude(x-axis) and rurality(y-axis)
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-4.png" alt="SHAP result" title="shap1">

#### SHAP Value of social economic factors for one county as an example
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-5.png" alt="SHAP result" title="shap1">

#### Plot bar graph to rank SHAP values for social economic factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-6.png" alt="SHAP result" title="shap1">

#### Beewarm graoh to rank SHAP values for social economic factors
<img src="https://github.com/Wenhuan2516/SHAP_Values_for_Suicide_Study/blob/main/shap-firearm-7.png" alt="SHAP result" title="shap1">
