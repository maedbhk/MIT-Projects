---
title: ClinicalBERT
---

> notes on paper by [Huang et al. 2019](https://arxiv.org/abs/1904.05342)

## What is clinicalBERT?
* ClinicalBERT is a flexible framework used to represent clinical notes. It uncovers high-quality relationships between medical concepts, as judged by physicians. 
* unstructured, high-dimensional and sparse information such as clinical notes are difficult to use in clinical machine learning models. 
* Clinical notes contain significant clinical value, compared to structured features, clinical notes provide a richer picture of the patient since they describe symptoms, reasons for diagnoses, radiology results, daily activities and patient history. Problem: for time-stretched physicians (example: those working in intensive unit) can't digest/compile all of the information presented across EHR, therefore, the question is: can a model do it for them? 
* Utility of clinicalBERT: actively predicting readmission has clinical significance, as it may improve efficiency and reduce the burden on intensive care unit doctors. 
* ClinicalBERT has developed a discharge support model that processes patient notes and dynamically assigns a risk score of whether the patient will be readmitted wtihin 30 days. 
* ClinicalBERT can also be adapted to other tasks such as diagnosis prediction, mortality risk estimation, and length-of-stay assessment. 

## How is ClinicalBERT different from other models? 
* Much of the previous work has used information at discharge whereas ClinicalBERT can predict readmission during a patient's stay.
* Makinga  prediction using a discharge summary at the end of hte stay means that there are fewer opportunities to reduce the chance of readmission. 
* ClinicalBERT predicts readmission at any timepoint since the patient was admitted. 
* Compared to two popular models of clinical text: Word2Vec and FastText, clinicalBERT more accurately captures clinical word similarity. 
* Where BERT is trained on BooksCorpus and Wikipedia, ClinicalBERT is also pre-trained on clinical notes.

## What does ClinicalBERT do?
* Learns deep representations of clinical text, which can uncover clinical insights (predictions of disease), find relationships between treatments and outcomes
* To evalute models on readmission prediction, a metric is defined based on a clinical challenge. 
* metric is alarm fatigue: useful classification rules for medicine have to have high positive predictive value (precision).
* **They evaluate model performance at a fixed positive predictive value** 
* They find that ClinicalBERT outperforms competitive deep language models. 
* Importantly, weights can be visualized to understand which elements of clinical notes are relevent to a prediction. 

## Questions:
* After pre-training, ClinicalBERT is fine-tuned on a clinical task (e.g. readmission prediction). What if someone wants to use another clinical task (length of hospital stay, mortality risk estimation), are those weights available? 
