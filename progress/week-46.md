---
title: Week 46
---

07/03/23 - 07/07/23

## Done and To Do
* Reached out to Ran Rotem (from marc weissopf's lab) about possible collaboration exploring prenatal determinants of mental health disorders
    * he gave a talk at the Picower conference on determinants of mental health
    * he used EHR and found that maternal hypothyroidism is associated with increased risk for asd in their children
    * my question is: can we identify an association between cerebellar injury prenatally (or shortly after birth) and later diagnosis of ASD? Structural neuroimaging work, and animal models have suggested that this association exists but no study has yet to leverage large-scale EHR data to corroborate this finding. 
* Met with Kseniia and Kai about item analysis project, trying out a few different approaches to map questions to responses
* Ran new HBN models on reading impairment data to try and answer some of the [questions](https://docs.google.com/document/d/1c06VE-7ONfemBjcVewU9VbH-NFTEcI4N6RpD2xaoFlU/edit?usp=sharing) that Ola outlined 
* Made progress on ADHD paper - ran a bunch of new models:
    * Differentiate kids with ADHD from all other kids WITHOUT adhd (target)
    * Differentiate kids with ADHD from all other kids with no diagnosis (target)
    * Does ML outperform simple sum scores  (features)
    * Removed subscores from models (features)
    * Check proprietary versus free questionnaires (features) - idea from kseniia
    * Predict general cognitive impairment score - revisited this analysis
    * Tried different algorithms: L1 and L2, logistic regression, decision tree, random forest etc. stochastic gradient descent linear classifier with L1 penalty, SGD with elastic net penalty, and linear support vector machine
    * Run secondlevel models on all models
    * To do: generalization to ABCD data
* Got access to Arcus yesterday so worked on that codebase yesterday and will work on it more today