---
title: Translational Neuroimaging
---

> Much of the points below came from a [review paper](https://www.nature.com/articles/nn.4478/) by Woo et al. (2017)

## Utility for pHealth
* Most translational neuroimaging studies have focused on diagnosis, identifing brain signatures that distinguish patients from healthy controls (if a model doesn't differentiate patients from controls or predict symptoms, it is unclear whether it is a clinically relevent model at all)
* Other models (although fewer in number) are being developed for more difficult classification and prediction problems, not easily addressed using existing clinical measures:
    * neuroimaging models for risk assessment
    * early detection
    * predicting conversion to full-scale disorders
    * differential diagnosis
    * sub-typing of patients and predicting treatment response

## Example Studies
* Alzheimer's Disease:
    * models have been able to predict who will later convert to a disease in advance of its onset. 
    * these models are possible because of ADNI dataset, which has collected longitudinal data from people with mild cognitive impairment (MCI)
    * the SPARE-AD index (spatial pattern of abnormality for recognition of early alzheimer's disease) is a particularly promising model. Specifically, the SPARE-AD model is a pattern classifier trained on spatial patterns of brain atrophy measured by structural MRI and indicates the presence of brain atrophy pattern, characteristic of AD. The model also predicts subsequent cognitive decline and transition to AD. 

## Differential diagnosis/subtyping and predicting outcomes
* neuroimaging models can also be used for differential diagnosis and patient subtyping (i.e. stratification): these models are useful because they can provide important information among disorders and symptoms at the biological level, potentially identifying subgroups that are not reflected in existing diagnostic categories. 
* many neuropsychiatric and neurological disorders are comorbid, therefore differential diagnosis can assist in identifying distinguishing features of neuropathology, and provide a new way to examine overlap across disorders. 
* some studies have successfully grouped patients into 'biotypes', which usually means that these patients have differential disease course or treatment response. For example a study by [Clementz et al. 2016](https://ajp.psychiatryonline.org/doi/full/10.1176/appi.ajp.2015.14091200) grouped patients with psychosis intro three transdiagnostic biotypes based on neuropsychology and EEG data, and another study by [Drysdale et al. 2016](https://www.nature.com/articles/nm.4246?TB_iframe=true&width=921.6&height=921.6) used resting state functional connectivity (rs-FC) to group patients with depression into 4 biotypes, based on differential responsiveness to transcranial magnetic stimulation. 
* Models are also built with the goal of customizing treatment based on individual brain markers: this endeavour is central to pHealth. For example: studies using brain measures to predict who will respond to a particular treatment can identify brain biotypes useful for guiding treatment. 

## What are next steps for translational neuroimaging? 
* modeling efforts must mature in order to provide clinically useful applications
    * diagnostic value: 
        * what qualifies a brain measure as being a sensitive marker? it must be diagnostic at the individual level. 
        * sensitivity refers to how robustly the measure responds when the outcome is present. 
        * specificity refers to whether the measure responds only in the presence of the target outcome and not to others. 
        * in moving from evaluating brain measures in a research to clinical settings, it is important to consider both positive and negative predictive values
        * what are the societal and clinical costs of false positives and negative errors?
    * deployability and scalability:
        * brain models that are useful for translation must be easily applicable to new individuals and shareable across groups
        * a recent (and encouraging) trend is named signatures for brain disorders. by naming neural signatures, it implies that models can be shared and annotated by many groups. one such example is SPARE-AD for Alzheimer's disease the PDRP (Parkinson's disease-related pattern)
    * generalizability 
        * models useful for translation must be generalizable in several ways: 1) they must generalize to new individuals, 2) the most useful signatures should generalize across laboratories, scanners, and minor variants in testing conditions, 3) useful signatures will generalize meaningfully to other outcomes related to the same construct. 
        * we need ecologically valid data sets. 

* Process-based predictive models:
    * most translational models are comprised of spatial patterns that map brain structure/function onto clinical outcomes. 
    * however, these models do not consider intermediate features or processes and are often minimally constrained by theories of brain function. 
    * they provide little description of the division of labor across brain regions and the dynamics of information flow through the regions included in the model. 
    * one promising direction is the development of signatures for basic mental processes - which can serve as intermediate features that are altered in various combinations of different disorders. 
    * these models are necessary if we're going to move beyond current diagnostic categories and establish specific forms of neuropathology that lead to specific functional problems across disorders (RDoC idea).