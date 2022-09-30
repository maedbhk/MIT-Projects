---
title: Methodological considerations for precision medicine
---

> All of the points below came from a [article](https://www.sciencedirect.com/science/article/pii/S0006322322016328) by Dhamala et al. (2022)

### Key Points
* data-driven ML can do the following:
    * identify disease-relevent biological subtypes
    * predict individual symptom profiles
    * identify shared and unique properties of diagnostic groups and associated symptom profiles.
    * recommend personalized therapeutic interventions
* in developing these tools, there are methodological considerations that need to be made
    * which algorithms are chosen?
    * which neuroimaging modalities and states?
    * data transformation, phenotypes, parcellations, sample sizes, populations
* in this review, the authors review applications of neuroiamging-based ML models to study psychiatric illnessess and discuss the effects of different methodological choices on model performance. 


### Introduction
* precision medicine is a powerful tool to understand clinical presentation at the individual-level by considering a range of biological and environmental factors. 
* in psychiatry, precision medicine and predictive modeling have two primary goals: 
    * discover how the brain gives rise to behavior
    * identify practically useful markers of behavior and clinical outcome. 
* what is different about precision medicine (compared to traditional medicine) is that it moves away from the one-size-fits-all model and seeks to identify the underying causes of disease and appropriate therapeutic interventions at a patient-specific level. 
    * specifically, ML can reveal neurobiological correlates of discrete and dimensional measures of psychopathology at the individual level.
    * ML can be used to generate individual-level behavioral predictions using descriptive, predictive, and prescriptive methods.
* precision psychiatry has the potential to transform how we diagnose and treat psychiatric illnesses. 

#### discrete and dimensional models of psychiatric illness
* discrete and dimensional models of psychiatric illness can provide complementary information. 
* discrete medical models can provide diagnostic labels based on clinical descriptions of signs and symptoms
* dimenionsal models typically describe broad hierarchical features of psychopathology

### Methods
* connectome-based predictive model (12) to predict behavior from connectivity data. for example, identify which connectivity features are most strongly correlated with a given phenotype, then using those features to build a linear model to predict behavior.
* BrainNet convolutional neural network (13) - maintains the topological complexity of brain networks, predicting future cognitive and motor development in preterm infants based on white matter connectivity
* benefits of these approaches - data-driven feature selection algorithms that do not rely on brain regions selected a priori, built-in cross validation (ensuring generalizabiity), continuous predictions that provide more dimensional measures of psychopathology
* individual differences in cognition, personality, as well as psychiatric diagnoses are thought to be most accurately predicted by functional connectivity, thus fMRI may be the best modality for predictive modeling. However, structural abnormalities associated with psychiatric disorders may also produce clinically informative predictions.

## Data transformation
* neuroimaging preprocessing pipeline and analytical methods can introduce variability into neuroimaging studies and subsequently bias findings.

## Phenotype selection
* clinically distinct phenotypic profiles can be assigned the same diagnosis - for both major depressive disorder and generalized anxiety disorder, inter-rater reliabilities are 0.28 and 0.21 respectively. 
* it is not realistic to think that the same neurobiological properties will underlie the unique clinical presentations of a given diagnosis.
* a further complication that impacts the clinical utility of brain-behaviorl models is that clinical scales can vary a lot in terms of the symptoms they capture, and single symptomatic or dimensional measures are insufficient to capture the complex nature of psychiatric illness in an individual. 

