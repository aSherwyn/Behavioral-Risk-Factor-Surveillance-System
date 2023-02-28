# Behavioral Risk Factor Surveillance System 2011-2021
![WCMS_home_image](https://user-images.githubusercontent.com/119871530/221697289-fbe53653-4911-42ae-a270-bb31040c3cde.png)

## Contents
- [About](#about)
- [Objectives](#objectives)
- [Features](#features)
- [Skills](#skills)
- [Process](#process)
- [Findings](#findings)
- [Logs and Dashboards](#logs-dashboards)
- [Data](#data)
- [Author](#author)
- [Footnotes](#footnotes)

## About <a name = "about"></a>

The Behavioral Risk Factor Surveillance System (BRFSS) is the Unites States’s premier system of health-related telephone surveys that collect state data about U.S. residents regarding their health-related risk behaviors, chronic health conditions, and use of preventive services. Established in 1984 with 15 states, BRFSS now collects data in all 50 states as well as the District of Columbia and three U.S. territories. BRFSS completes more than 400,000 adult interviews each year, making it the largest continuously conducted health survey system in the world.

By collecting behavioral health risk data at the state and local level, BRFSS has become a powerful tool for targeting and building health promotion activities.

However, as comprehensive as the BRFSS is, it is equally overwhelming in magnitude and variety. It covers topics from dietary habits to alcohol use to prostate exam frequency. Responses are stratified into multiple categories such as age, ethnicity, state, and year. Official categories, responses, and questions vary from year to year. **In this project I cleaned years 2015-2021, wrangled and uploaded more approachable subsets to kaggle, and conducted analyses by state, country, and demographic categories for the following questions**[[1]](#f1).

## Obectives <a name = "objectives"></a>
- [x] Gain a functional understanding of the BRFSS and its variables.
- [x] Creat subsets of the original dataset and upload for public use.  
- [ ] Provide current regionally relevant health metrics to healthcare professionals and policy makers.
- [ ] Provide current demographically focused health metrics to healthcare professionals and policy makers.
- [ ] Examine the impact of COVID-19 on general health, mental health, and dietary health, and physical fitness.

## Features <a name = "features"></a>
<a href="https://github.com/aSherwyn/Behavioral-Risk-Factor-Surveillance-System/blob/main/03%20Scripts/01%20Cleaning.ipynb">`Thorough cleaning process with detailed, color-coded notations throughout.`
![Screenshot (302)](https://user-images.githubusercontent.com/119871530/221743647-73003bc5-f3d1-4f65-9b6a-b86cbab9208f.png)</a>


<a href="https://github.com/aSherwyn/Behavioral-Risk-Factor-Surveillance-System/blob/main/03%20Scripts/02.3%20Overall%20Health%20by%20State%20-%20Correlations.ipynb">`Correlation heatmaps with strong, moderate, and weak sub-maps as well as category-specific heatmaps.`  
![download](https://user-images.githubusercontent.com/119871530/221739020-d66efe01-1262-4d65-be3b-2a1a08777418.png)</a>

<a href="https://github.com/aSherwyn/Behavioral-Risk-Factor-Surveillance-System/blob/main/03%20Scripts/02.5%20Overall%20Health%20by%20State%20-%20Linear%20Regressions.ipynb">`Linear Regressions and correlating statistics plotted and calculated via elegant user-defined functions to optimize reusability and task duration.`</a>  
```python
# This function will plot a linear regression and print the statistics
# of a variable against a list of variables.

def reg_plot(x_name, y_list, threshold):
    for i in range(0,len(y_list)): # Making for loop to run through y_list
        
        y_name = y_list[i] # Defining y_name variable from y_list iteration
        
        df_temp = df[[x_name, y_name]].copy() # Creating a temporary dataframe
        df_temp.dropna(inplace = True) # Cleaning the temporary data frame
        ...
```

<a href="https://github.com/aSherwyn/Behavioral-Risk-Factor-Surveillance-System/blob/main/03%20Scripts/02.6%20Overall%20Health%20by%20State%20-%20Geospatial%20Analysis.ipynb">`Combined for loops and user-defined functions to plot category-specific maps from a geopandas dataframe.`</a>
```python
# Plotting maps for all the BMI category variables

map_list = ['BMI: Obese (BMI 30.0 - 99.8)',
              'BMI: Overweight (BMI 25.0-29.9)',
              'BMI: Normal Weight (BMI 18.5-24.9)',
              'BMI: Underweight (BMI 12.0-18.4)']

for m in map_list:
    plot_map(m)
```

## Skills <a name = "skills"></a>

## Process <a name = "process"></a>

## Logs and Dashboards <a name = "logs-dashboards"></a>
- [Project Log](https://github.com/aSherwyn/Behavioral-Risk-Factor-Surveillance-System/blob/main/04%20Analysis/BRFSS%20Project%20Log.xlsx)

- Health Across the Nation Dashboard
- BMI Dashboard
- Dietary Health Dashboard
- General Health Dashboard
- Mental Health Dashboard
- Physical Activity Dashboard

## Data <a name = "data"></a>
**Original Data:**  
[CDC's BRFSS Data](https://chronicdata.cdc.gov/Behavioral-Risk-Factors/Behavioral-Risk-Factor-Surveillance-System-BRFSS-P/dttw-5yxu)  
[BRFSS Methodology](http://www.cdc.gov/brfss/factsheets/pdf/DBS_BRFSS_survey.pdf)  
[BRFSS Glossary](https://chronicdata.cdc.gov/Behavioral-Risk-Factors/Behavioral-Risk-Factor-Surveillance-System-BRFSS-H/iuq5-y9ct/data)  

**Wrangled Datasets:**  
[BRFSS Overall Health by State 2015-2021](https://www.kaggle.com/datasets/asasherwyn/brfss-overall-health-2015-2021)  
[BRFSS Dietary Health 2015-2021](https://www.kaggle.com/datasets/asasherwyn/brfss-dietary-health-2015-2021)  
[BRFSS General Health 2015-2021](https://www.kaggle.com/datasets/asasherwyn/brfss-general-health-2015-2021)  
[BRFSS Mental Health 2015-2021](https://www.kaggle.com/datasets/asasherwyn/brfss-mental-health-2015-2021)  
[BRFSS Physical Activity 2015-2021](https://www.kaggle.com/datasets/asasherwyn/brfss-physical-activity-2015-2021)  

## Author <a name = "author"></a>
**Asa Sherwyn, Data Analyst<br>**
<a href="https://www.linkedin.com/in/asasherwyn/"><img src="https://user-images.githubusercontent.com/119871530/221632937-e4763ba3-68a5-4aa5-9e4c-dbf067d910fa.png" width="20" height="20" target="_blank"></a>
<a href="https://kaggle.com/asasherwyn"><img src="https://user-images.githubusercontent.com/119871530/221633194-02c8302c-8f12-420c-b3af-977790c57cd6.png" width="20" height="20" target="_blank"></a>
<a href="https://public.tableau.com/app/profile/asa.sherwyn"><img src="https://user-images.githubusercontent.com/119871530/221633938-eb92c3af-647d-48a6-9fa5-8900bfd44cc0.png" width="20" height="20" target="_blank"></a>
<a href="http://asherwyn.github.io/"><img src="https://user-images.githubusercontent.com/119871530/221634877-471e1fd4-e3bc-41c3-b3e7-ca158e8659fb.png" width="20" height="20" target="_blank"></a>

## Footnotes <a name = "footnotes"></a>
[1] <a name = "f1"></a>**Questions used in the subsets and analysis for this project:**
  - How is your general health? `BRFSS QuestionID: GENHLTH`
  - Weight classification by Body Mass Index (BMI) (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _BMI5CAT`
  - Health Status (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _RFHLTH`
  - About how long has it been since you last visited a doctor for a routine checkup? `BRFSS QuestionID: CHECKUP1`
  - Days when mental health status not good (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _MENT14D`
  - Do you have serious difficulty concentrating, remembering, or making decisions? `BRFSS QuestionID: DECIDE`
  - Consumed fruit less than one time per day (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _FRTLT1A`
  - Consumed vegetables less than one time per day (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _VEGLT1A`
  - During the past month, did you participate in any physical activities? (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _TOTINDA`
  - Participated in 150 minutes or more of Aerobic Physical Activity per week (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _PAINDX2`
  - Participated in enough Aerobic and Muscle Strengthening exercises to meet guidelines (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _PASTAE2`
  - Participated in muscle strengthening exercises two or more times per week (variable calculated from one or more BRFSS questions) `BRFSS QuestionID: _PASTRNG`
