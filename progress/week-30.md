---
title: Week 30
---

03/12 - 03/17

## Done and to-do
* Alyson paper: New models with SMOTE + full demos + all features (Parent/Child/Teacher) to classify sex and ADHD diagnosis
    * worked on unsupervised learning (UMAP) to subtype ADHD + Sex (nothing concrete yet..)
* HBN + fMRIPrep: wrote preprocessing script to incorporate SUIT derivatives into fMRIPrep output
    * plan on running [xcp](https://xcp-d.readthedocs.io/en/latest/) as post-processing for some of the HBN particpants, interested first in parcellating data using Yeo/Buckner (7,17) parcellations for cortex and cerebellum, will run on a subset of participants with ADHD
* HBN phenotype models: working with Shreya to incorporate multi-label classification into pydra-ml so that we can predict multiple diagnoses (and subtypes) rather than binary of diagnosis/no diagnosis
* To-do: run HBN models that do not contain total/overall scores per questionnaire. This is a bit tricky as these overall scores are coded differently across questionnaires, perhaps this will be made easier by moving HBN to reproschema. [Hired an RA (freshman CS)](../mentorship/spr23_urop_onboarding.md) to work on this project. 
* Met with Lexi to discuss [ADHD + Professions project](../projects/adhd_professions.md). [Hired an RA (freshman CS)](../mentorship/spr23_urop_onboarding.md) to work on this project. 
    * We want to use the method employed [in this paper](https://www.nature.com/articles/s41598-022-12905-y) in which they convert UK SOC 2000 codes (from the UK Biobank) into [U.S. SOC/O*NET job](https://onlinelibrary.wiley.com/doi/epdf/10.1111/j.1744-6570.2001.tb00100.x) titles using Computer Assisted Structured Coding Tool [CASCOT](https://warwick.ac.uk/fac/soc/ier/software/cascot/). The data for both of these datasets are publicly available (UKBiobank requires DUA) however the authors (when contacted) were unwilling to share either the data or the code. We've emailed back and forth a few times but haven't had much luck so far, something to discuss when we next meet. It would be really useful for this project to have the traits and attributes (e.g., innovation, complexity) associated with UK Biobank occupations. 