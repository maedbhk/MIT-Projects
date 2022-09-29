---
title: Neurodevelopment and Translational Neuroimaging
---

> Much of the points below came from a [article](https://www.sciencedirect.com/science/article/pii/S0960982220301585) by Siugzdaite et al. (2020)

## Introduction

* 14-30% of children/adolescents live with a learning-related problem, associated with cognitive/behavioral problems. examples of these disorders are dyslexia, dyscalculia, language disorders. other diagnses related to neurodevelopmental disorders are adhd, asd. 
* how does the developing brain give rise to disorders? 
* there has been a lot of inconsistency in ascribing a range number of brain regions to individual neurodevelopmental disorders. 
* for example: adhd has been associated with grey matter differences within ACC, caudate nucleus, pallidum, striatum, cerebellum, PFC, premotor cortex etcs.
* why does this inconsistency exist? diagnostic groups are highly heterogeneous and overlapping and symptoms vary a lot within categories. there is no "purity" of developmental disorders. 
* solution: transdiagnostic approach?
    * What is transdiagnostics? 
    * Identifying underlying symptom dimensions that span multiple diagnoses.
    * for example, within neurodevelopmental learning disorders, primary focus is on identifying cognitive symptoms that underpin learning. 
* another reason for inconsistent brain-to-cognition mappings: they do not exist!
    * equifinality: there could be many possible neural routes to the same cognitive profile or disorder
    * multifinality: the same local neural deficit could result in multiple different cognitive symptoms across individuals.
    * these concepts have not yet been translated into analytic approaches. 

### Goal of the study
* take a transdiagnostic approach to establish how brain differences relate to cognitive difficulties in childhood
* how can the same pattern of neural deficits result in different cognitive profiles across children? 

### Method
* cognitive data from children with and without diagnoses were entered into an unsupervised ML algorithm called an artificial neural network -- which preserves information about profiles within the dataset, captures non-linear relationships, and allows for measure to be differentially related across the sample. ideal method to use with transdiagnostic cohort. 
* to determine how brain profiles relate to cognitive profiles, the same ANN was applied to whole-brain cortical morphology data
* Artificial neural network: cognitive data (z scored): age standarization mean and standard deviation from each assessments
* specific type of network: self-organizing map - this algorithm represents multidimensional datasets as a two-dimensional map. 

* Cognitive profiles are robustly related to children's learning ability, so a good test of whether the network can reliably represnt individual differences in cognition is to test whether it will generalize to unseen data and predict children's learning scores.

* Mapping brain profiles: 
* Whole-brain cortical morphology metrics (cortical thickness, gyrification, sulci depth) were calculated for each child across a 68 parcel brain decomposition. 
* Feature selction was performed before machine learning to reduce the risk of over-fitting with so many measures. 
* LASSO regression reduced the number of indices down to 21 distint measures

### Results
* summary of results: 
    * hold out CV revealed that cognitive profiles learned using ANN generalized to unseen data and were sig. predictive of childrens' learning difficulties
    * similarly, hold out CV showed that brain profiles generalized to unseen data and a child's age-corrected brain profile was sig predictive of age-normed cognitive profile.
* there were no one-to-one mappings: one brain profile could be associated with multiple cog profiles and vice versa
* also, researchers found that the more central the hubs to a child's brain organization, the milder or more specific the cognitive impairments. when these hubs were less well embedded, children showed the more severe cognitive symptoms and learning difficulties. 
* children's brain profiles predict their cognitive profile. 

#### What is the artificial neural network learning? 
* is it learning about the severity of a particular set of brain values, or whether it had learned to identify peaks and troughs in individual profiles? 



