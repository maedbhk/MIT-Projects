---
title: Roundtable: maximizing the clinical utility of small-scale neuroimaging studies
---

### Benefits, limits and pitfalls of large data approaches - Simon Eickhoff
* individual predictions from neurobiology
	* just larger n is not all that is needed, train on large and underrepresented populations
* precision medicine for brain disorders
	* be careful with this approach.
* long road to practical utility 
	* very long road to practical utility, where a patient actually has a real benefit
	* data collected from large hospitals may not work on community sample
	* models love short cuts. regress out age, sex, body size - nothing else is left. 
	* short cut that the model has learned may turn into a dead end street
* confounds, bias and discrimination

### maximizing utility in small-sample psychiatric samples
* predict future timepoints
* power dynamics change
* prediction target matters - engage people with lived experiences in choosing a target variable
* target: function/symptoms/familial ties not symptoms etc. functional outcomes are really important, which map on to neurobiology better than symptoms
* lived experience is important, and of love ones. learn/loved/labor experiences - domain knowledge in psychiatry
* Kilackey (2023), published in lancet
* clinicians will put more emphasis of n=60 trial than n=6000 trials. Meet clinicians where they are instead of pumping out large observational studies. 
* boost accuracy in small samples by leveraging large samples (metamatching). Yeo et al. train model on large dataset and then go to another dataset. (to boost performance in small psych samples)
* what is the R value of this disorder that would be relevant? ask clinicians, meet them where they are.

### Mechanism as a goal of clinical prediction
* carefully consider outcomes of interest - define question. identify clinical population define treatment response. 
* select timing of fMRI - pre-tx, early in tx, post-tx. define window of assessment
* collect baseline data, acquire neuroimaging data, acquire baseline clinical data. 
* collect longitudinal data - measure substance use over time, collecte treatment-related measures. 
* evaluate model, understand results, improve clinical care. 

### densely sampled neuroimaging and phenotypes
* dense sampling as big data
* heterogeneity as noise vs. as dynamic signal
	* within-person study, how do variables co-vary together? distinguish between noise and state
	* a lot of psychiatric disorders are dynamic, do within-person studies ... (treatment, transitions etc.)
	* precise, individualized data - picture of a person's phenotypes or behavioral data. 
* clinical implications

### how can we capture individual differences w/multi-modal data (including fMRI)
* concerns about fMRI:
	* low reliabilty
	* required large sample size
	* better approaches for fMRI: dynamic states within a single person
		* ML/AI can help but not as much as you may think
		* better "features" - assays and probes, movie-watching instead of resting state
	* computational/behavioral phenotypes for predictions
		* behavioral features often outperform neuroimaging features
		* latent neurocognitive features
		* bayesian optimal design (adaptive design optimization)
		* theory-driven and data-driven
		* real-time / real-world paradigms


