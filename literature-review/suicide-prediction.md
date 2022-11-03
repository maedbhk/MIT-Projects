---
title: Suicide prediction using structured-unstructured interactions in EHR models
---

> Ideas from [Bayramli et al. 2022](https://www.nature.com/articles/s41746-022-00558-0)

### Goals of Research
* Unstructured EHR have been used for clinical predictive tasks, both as a standalone feature-set and in combination with structured data
* ultimate goal: optimally integrate both data types to improve predictive performance. 
    * 1) compare the predictive value of structured and unstructured EHR data as standalone datasets for predicting suicide risk
    * 2) evaluate the increase in prediction performance when integrating both structured and unstructured data using various models
    * 3) identify structured-unstructured feature pairs in which the interaction between the two features differs substantially between case + non-case populations

### Challenge
* predicting suicide risk is a complex challenge. Clinicians' intuition for detecting at-risk individuals is no better than random chance. 

### Methods:
* structured data: diagnoses, labs, medications, procedures
* unstructured data: clinician notes
* contingency analysis: joint suicide attempt of risk features A (structured) and B (unstructured) is defined as the log of the ratio of the expected joint occurences of AB in suicide vs. non-suicide group
* models: 
    * ***naive bayes classifier (NBC)*** - subclass of bayesian networks that assume strong conditional independence of all input features, greatly reducing model complexity. well-suited for clinical decision support tasks - highly scalable and interpretable. they compute a risk score for each concept using the odds ratios of its prevelence in case and non-case populations. During validation, the NBC risk scores for each concept in a patient's visit history were added together to compute a cumulative suicide risk measure for the subject. 
    * ***balanced random forest classifier*** - capable of capturing interactions between features. Balanced random forests are an extension of random forest models and work well with label-imbalanced datasets. 

### Findings:
* models trained only on features derived from structured-data perform better than mdoels trained only on features derived from unstructured data. 
    * but importantly, the performance gap between models trained with structured data and those trained with unstructured data is quite small, especially considering the compact size of the unstructured data
* unstructured data may help capture complementary information about the well-being of patients that structured data may not provide (e.g., environmental risk factors: living on the street, prisone etc.)