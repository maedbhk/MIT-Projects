---
title: UK Biobank
---

## [UK Biobank](https://www.ukbiobank.ac.uk/)

### Overview 
UK Biobank is a large-scale biomedical database and research resource, containing in-depth genetic and health information from half a million UK participants. 

* Population: 
* Data collected:
    * Population: M/F ages 9-65
* **Online questionnaire data** (n=330,000)
    * Diet, cognitive function, occupational history, mental health, digestive health, chronic pain, food preferences, neurodevelopmental issues, sleep, pain
* **Genetic data**
    * Whole genome sequencing data (n=200,000), whole exome sequencing data (n=450,000)
* **Health-related outcomes data** (n=230,000)
    * Primary care data containing coded clinical events (consultations, diagnoses, procedures, laboratory tests), prescribed medication (referrals) - info on Covid-19 now.
    * Hospital inpatient data - diagnosis, date of admission, underlying conditions, discharge information. 
    * First occurrences of medical conditions
    * Death data
    * Cancer data  
* **Imaging data** (n=50,000)
    * MRI (DTI maybe?) also scans of other body parts: liver, muscle, heart, abdomen
    * Post-covid scans on n=2000 participants
* **Baseline data** (n=500,000)
    * Measurements, hand grip, spirometry, bone density
    * Blood, urine, saliva, 
    * Diet preferences
* **COVID-19 data**
    * MRI scans on n=2000 participants, what else has been collected?
* **Blood + Urine** (n=500,000)
    * Saliva for 100,000
* **Activity Monitor** (n=100,000)
    * Physical activity data over a 7-day period collected via a wrist-worn activity monitor 
* **Biomarker data** (n=500,000)
    * Also n=20,000 who completed a 4-5 year follow-up assessment. 
    * 34 biomarkers chosen (e.g., HbA1c for diabetes).
    * Blood count (hematological assays)
    * Infectious disease markers
    * Metabolomic biomarkers
    * Telomere length

### Data Storage - Questions
* Which data are on openmind?
    * Imaging (rest, task, naturalistic)
    * Demographic info
    * Cognitive/Behavioral results
    * Clinical disorders
* What is the format?
    * raw, derivatives
* Have imaging (MRI/fMRI) data been preprocessed?
    * fmriprep
    * freesurfer
    * first-level glms
* Where are the data stored on openmind?
    * are these data being transitioned to datalad?
* How does a new user get access to the dataset?

### Data on OpenMind
* Phenotypic data are stored here: `/om2/user/maedbh/ukbiobank_data`
    * All data are saved in **ukb670488.csv**
    * Data dictionary are saved in **ukb670488.html**