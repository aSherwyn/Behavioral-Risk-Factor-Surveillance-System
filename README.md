# Behavioral Risk Factor Surveillance System Analysis 2011-2021

The Behavioral Risk Factor Surveillance System (BRFSS) collects survey responses to hundreds of general health questions from 400,000 respondents annually. This project aims to clean, wrangle, and analyze this data to provide a better understanding of its contents. I used Python and Tableau to process and present the BRFSS’s 2.1 million records.

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

However, as comprehensive as the BRFSS is, it is equally overwhelming in magnitude and variety. It covers topics from dietary habits to alcohol use to prostate exam frequency. Responses are stratified into multiple categories such as age, ethnicity, state, and year. Official categories, responses, and questions vary from year to year. **In this project I cleaned years 2015-2021, wrangled and uploaded more approachable subsets to kaggle, and conducted analyses by state, country, and demographic categories for the following questions**[^1].

## Obectives <a name = "objectives"></a>
- [x] Gain a functional understanding of the BRFSS and its variables.
- [x] Creat subsets of the original dataset and upload for public use.  
- [ ] Provide current regionally relevant health metrics to healthcare professionals and policy makers.
- [ ] Provide current demographically focused health metrics to healthcare professionals and policy makers.
- [ ] Examine the impact of COVID-19 on general health, mental health, and dietary health, and physical fitness.

## Features <a name = "features"></a>

## Skills <a name = "skills"></a>

## Process <a name = "process"></a>

## Logs and Dashboards <a name = "logs-dashboards"></a>
- Project Log

- Health Across the Nation Dashboard
- BMI Dashboard
- Dietary Health Dashboard
- General Health Dashboard
- Mental Health Dashboard
- Physical Activity Dashboard

## Data <a name = "data"></a>
**Original Data:**  
[BRFSS Data](https://chronicdata.cdc.gov/Behavioral-Risk-Factors/Behavioral-Risk-Factor-Surveillance-System-BRFSS-P/dttw-5yxu)  
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
[^1]Questions used in the subsets and analysis for this project:
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
