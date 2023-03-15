---
title: ADHD + Professions
---

## Question
* Is there a relationship between the type of occupation someone holds and whether or not they have ADHD?
    * The hypothesis is that people with ADHD are more likely to hold jobs that have the following traits/attributes: short-term planning, entrepreneurship, creativity, flexibility, self-employment. Job status will also be modulated by the following demographic variables: race/ethnicity, sex, age, socioeconomic status (SES)
* Occupation will be coded by the following attainment phenotypes: complexity, autonomy, innovation, and three types of job demands (information demands, emotional demands, and physical demands
![occupational phenotypes](https://www.nature.com/articles/s41598-022-12905-y/tables/1){fig-align="center"} based on the method outlined by [Song et al. 2022](https://www.nature.com/articles/s41598-022-12905-y#Sec13)

## Dataset
* [**UK Biobank**](https://www.nature.com/articles/s41586-018-0579-z.) cohort is a population-based cohort study in the United Kingdom, which involves above 500,000 participants aged 40 years or older during their recruitment between 2006 to 2010
* In the UK Biobank data, participants’ jobs were coded using the four-digit UK Standard Occupational Code (SOC) 2000 (Field ID 132) based on detailed job information (e.g., job tasks and activities) collected during participants’ baseline visits to assessment centers for the discovery sample
    * [additional reading](https://www.nature.com/articles/s41586-018-0579-z.)
* [**ONET**](https://onlinelibrary.wiley.com/doi/epdf/10.1111/j.1744-6570.2001.tb00100.x) is based on the U.S. SOC system and includes hundreds of job characteristic measures for over 1100 occupations, sufficiently representing the national labor force in the United States, and has been used in many other countries via similar occupational classification systems
    * [additional reading](https://onlinelibrary.wiley.com/doi/epdf/10.1111/j.1744-6570.2001.tb00100.x)

## Method
* First, convert UK SOC 2000 codes into U.S. SOC/O*NET job titles using Computer Assisted Structured Coding Tool [CASCOT](https://warwick.ac.uk/fac/soc/ier/software/cascot/)
* Second, manually check and match occupations in these two systems based on detailed job descriptions (e.g., job tasks and activities), based on the International Labor Organization’s International Standard Classification of Occupations (ISCO) to ensure accuracy and reliability of the crosswalk in the first step. 
* For the 502,538 participants, you should be able to match ONET job titles for 274,223 individuals. The remaining 192,010 individuals who did not provide SOC codes and 36,305 who had SOC 2000 codes but no sufficient information to match the O*NET job titles should be excluded.
* For full methods details, see Section **Materials and methods - Phenotype measurement and definitions** in paper by [Song et al. 2022](https://www.nature.com/articles/s41598-022-12905-y#Sec13)