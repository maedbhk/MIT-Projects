---
title: Week 9
---

## Done and To Do
*  Onboarded two research assistants, here is the updated [onboarding document](../mentorship/fall22_urop_onboarding.md) and orientation to [openmind](../openmind/setup.md)
* some interesting observations from predictive modeling of hbn phenotypic assessments, you can look through the models in this [notebook](../notebooks/phenotype_models.html)
    * models are trained on different feature sets (decision tree classifier) and the target is whether a participant has/has not been diagnosed with a disorder
    * Some observations: 
        * achievement vs intelligent gap such that intelligence is not a predictor of whether or not someone is diagnosed with a developmental disorder, but achievement is
        * many parental questionnaires are not useful in predicting outcome, for example, financial support, social status, basic demographics. Questionnaires that are relevent concern questions related to mood and feelings, anxiety etc. 
* have also observed feature importances for each of these models (along with permutation importance) - have not yet analyzed any of these features in depth, will be tasking research assistants with these next steps, particularly to investigate model predictions for specific subgroups, focusing on adhd + autism, and anxiety + mood disorders. One follow-up question I have is related to the achievement and intelligence prediction gap, and whether this is predominately driven by the children diagnosed with adhd. 
* have been working on pyBIDS + SUIT, figuring out how best to integrate matlab + python code. spent some time researching and building singularity containers (more involved than anticipated). 
* will work with Jeff to analyze some of the naturalistic data for HBN rather than resting state. In terms of SNR, I would rather start building connectivity models with movie data than resting state data. almost ready to run SUIT pipeline on larger subset of HBN participants, focusing on adhd + autism, anxiety + mood disorders. 
* broader connectivity question will focus on PFC-cerebellar connectivity across these sub-groups and across developmental stages, identifying whether changes in connectivity can predict clinical characteristics of these disorders, and if so, how these differences arise across the developmenal span.

## Questions
* Meeting with Jaan the week of Oct. 17th to discuss [this paper](https://arxiv.org/abs/1904.05342), which should be relevent to CHOP project. I suggested our Wednesday meeting time so we could meet all three of us if that works for you? If that time doesn't work for him, I can suggest 11am on Monday? 
