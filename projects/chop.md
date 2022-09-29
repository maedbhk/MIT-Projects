---
title: CHOP Project
---

## Datasets
* CHOP emergency department: 
    * What does this dataset contain? 
        * Behavioral Health screen - psychometrically developed by a company and used by CHOP since 2014 to give staff in the ER a sense of mental health burden for each child. Questions include environmental adversity and other data that are difficult to collect. Demographics are included.
        * They also have regular EHR - which I believe are medical notes made by clinician.
        * Geocoded level data (which neighborhoods etc. environemental triggers)
    * Dataset summary:
        * n = 20,000 children, ages 14-18
        * 50% of sample are Black
        * prevelence of suicide attempt is 50%
        * 15% of the cohort have longitudinal data
        * 2500 children with two timepoints, 1500 with 3 or more timepoints
        * data have also been collected before and during covid, so this is another variable that could be of interest
        * no guarantee that any information from the past will be include about developmental disorders (whatever is shared by children)
    * questions:
        * which features are predictive of suicide attempt? drug use, bullying etc.
        * are there environmental factors contributing to suicide attempt? 
        * what are the comorbidites of this sample? 
        * how does suicidality aspect relate to p factor (what is p factor?)
    * goals:
        * with suicidality, comorbidities are the rule, not the exception
        * classification algorithms are good because they have clinical application and are interpretable
        * causal effects are target now for intervention
* MRI dataset
    * what does this dataset contain? 
        * structural data is collected clinically but not functionally. in total, there are about 100,000 scans at CHOP but many of the participants in the clinical dataset likely don't have MRI scans. 
        * there are also neonatal scans: 0-2 years of age + preterm children. 
        * large subset of children have 22Q (22q deletion syndrome) can affect any system of the body, however, most children wtih 22q have heart, immune, learning, speech, and/or behavior difficulties.
* Standarizing radiological reports
    * radiological notes are still transcribed by people, use AI to translate

### Project Goals
> Ideas from [Czyz et al. 2021](https://journals.sagepub.com/doi/full/10.1177/1073191120939168?casa_token=nZwwu0a6mM4AAAAA%3AUE4tkOVOBDe0BEXfvZDRMFSH-BjpA4Cq07RRlY9s_cZsfePwk9W9nE3Odc4qW9qh5UW5lCs4qj3dcA)
* Can we identify reliable proximal markers of suicide risk to inform personalized interventions provided at crucial moments in the individual's natural environment?    
    * Validated indicators of proximal risk could lead to the development of adaptive interventions
    * Short-term risk prediction is a key concern for clinical providers and more research that incorporates proximal assessment is needed to provide insights about short-term precursors to  suicidal ideation in order to facilitate early detection of risk as well as inform targeted interventions.
* Are existing tools/models validated on diverse communities of adolescents? 
    * There is a great need to ensure that screening tools serve youth from diverse backgrounds, identities, and cultures. 
* One major goal of this work would be to integrate screening into clinical practice. 
* Are there environmental predictors of suicide risk? Can this be identified using geocoded data? 
* Was covid a risk factor of suicide attempt? 

### Questions for CHOP team 
* Both Satra and I have received NTP approval -- what are next steps with regard to data access? 
* Is there a CHOP cluster for running scripts? If so, how do we get access? 
* Even before looking at data, could we get an example of the behavioral health screening questionnaire? 
* Can we confirm the types of data collected for the sample of 20,000 adolescents: BHS, demographics, geocoded information (zipcodes?), anything else I'm missing?  
