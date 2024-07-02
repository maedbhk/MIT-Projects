---
title: Brain connectivity and clinical application
---
### Overview
Organized by molecular connectivity group (molecularconnectivity.com)
* fMRI has been around for a long time, still no clinical application? 

### Simon Eickhoff
* classical biomarkers relies on within-sample comparison or association (patients vs. controls)
	* problem: misleading biomarkers -also pertain to group means. individual statements are usually not possible
	* changing in the context of machine learning, key conceptual point, not testing for group means, train model on available data (some multivariate features) - does model generalize? 
* preprocessing, compression, target of ML approach matters for predictive accuracy
* compound scores tend to be more reliable than individual scores
* how well can you actually predict your targets just by looking at non-brain markers? (SES etc.). Too much emphasis on connectome prediction without considering other phenotypic markers? 
* human variability is likely low-dimensional:	
	* confounds are a gradient and perhaps everything is a confound
	* no such thing as a deconfouned analysis

### ??
* investigate training N dependence on out-of-sample prediction of endpoints for standard inter-subject covariance analysis
	* at what point does adding more data fail to result in any predictive/explanatory gain? 
* investigate topographic robustness of derived pattenrs - another metric apart from endpoint prediction -> important for understanding mechanisms
* META or MEGA analysis: is it better to use all available data in one shot, or split the data into parcels? 
* Inter-individual (rather than intra-individual)
* analysis framework: scaled subprofile modeling (=SSM), form of PCA regression
	* step 1: PCA on fMRI data
	* brain-behavior modeling
	* construction of corresponding brain pattern
	* application of brain behavioral model to held-out data
* big picture synthesis and caveats
	* increasing N in the training sample beyond N=o(1000) does not result in any predictive gain for "shallow" techniques and group-level pattners (flip side ot marek et al. 2022)
	* both large trianing and test samples will show increasing sig. for fixed effect sizes - no real scientific insight
	* tension between prediction and explanation (yarkoni paper)


### ??
* decoding fMRI (dys)connectivity via cross-species fMRI
* functional networks - mouse brain - better understanding of mechanisms
	* fMRI connectivity difference, 20 different mutations
* functional and structural connectivity are closely related
* does fMRI hypoconnectivity reflect reduced axonal input? 
* can you silence activity in one region and then observe hypoconnectivity? 
* methods: chronic silencing of DMN chronically and actutely (overexpress sodium channel)
	* difference: more connectivity when DMN has been chronically silenced (regions that have strong projections from PFC)
* less is more: cortical silencing results in fMRI hyperconnectivity 
* increasing excitability of the mouse PFC with chemogenetics
* excitation results in fMRI hypoconnectivity 
* fMRI connectivity is dominatd by changes in slow/infraslow neural coherence (faster to slow, not fast rhythms)

## Deobra Peretti
* what is needed from a clinical perspective? 
	* reliable measurements
	* simple and integrated softwares
	* healthy databases
	* single-subject metrics
		* most molecular imaging is done on group measures
	* scaled subprofile modelling using PCA
		* generation of characteritic disaes patttern, gives each subject a score that characterizes disease expression, can be used to test new subjects
		* examples from PD, AD, SCA
	* parksinson's disease pattern
	* in clinical practice, move from clinical profile to biomarker profile, so as not to rely on the practioner (??)
	* methodological issues:
		* SSM/PCA is sensitive to scanner, acquisition protocols, image processing